Project 2: System Design Class; Study Session Tracker

The following is the entire Copilot chat history I conducted in VSCode:






NatashaAlv: simplify the following so as to resemble a proper prisma schema to replace the current model in schema.prisma 
avoid spaces in field names

{
  "_id": {
    "$oid": "6931d1cbb07df358ed6f9101"
  },
  "Date": {
    "$date": "2025-12-04T05:00:00.000Z"
  },
  "Subject type": "Art",
  "Class Name": "System Design",
  "Time Estimate (h)": 3,
  "Start Time": "8am",
  "Session Goal": "start working on project",
  "Productive Time (h)": 1,
  "Distracted Time (h)": 4
}

GitHub Copilot: I'll read the current schema and then replace it with a simplified Prisma model based on your data structure. 

Read [](file:///Users/sinnacado/Desktop/Project-2/prisma/schema.prisma)

Now I'll replace the model with a proper schema based on your data structure: 

Using "Replace String in File"


```

```
Done! I've replaced the schema with a model that matches your data structure. The model:
- Uses camelCase for field names (no spaces)
- Maps to your original MongoDB field names using `@map()`
- Keeps the collection name as "sessions" with `@@map()`
- Uses appropriate types (DateTime, String, Int)
- Maintains the ObjectId for the `_id` field

Made changes.

NatashaAlv: remove the @map elements

GitHub Copilot: Using "Replace String in File"


```

```
Done! All `@map()` directives have been removed from the schema.

Made changes.

NatashaAlv: update the html form so that all fields in the schema are represented. remove the cat fields from the form

GitHub Copilot: Using "Replace String in File"


```

```


Using "Replace String in File"


```

```
Done! The form now includes all fields from your Session schema:
- date (date picker)
- subjectType (text input)
- className (text input)  
- timeEstimateH (number input)
- startTime (text input)
- sessionGoal (textarea)
- productiveTimeH (number input)
- distractedTimeH (number input)

All cat-related fields have been removed, and the UI text has been updated to reflect study session tracking.

Made changes.

NatashaAlv: update the renderItem function to show sessions instead of cats

GitHub Copilot: Using "Replace String in File"


```

```


Using "Replace String in File"


```

```


Using "Replace String in File"


```

```


Using "Replace String in File"


```

```
Done! The `renderItem` function now displays study session data instead of cat data. The card shows:
- Class name and subject type in the heading
- Date and start time
- Time estimates (estimated, productive, and distracted hours)
- Session goal

I've also updated the related text references from cats to sessions throughout the script.

Made changes.

NatashaAlv: configure git globlly for user with emial "alvarnat@sheridancollege.ca". and Name Natasha Alvarado Dubkova 

GitHub Copilot: Ran terminal command: git config --global user.email "alvarnat@sheridancollege.ca" && git config --global user.name "Natasha Alvarado Dubkova"

Done! Git is now configured globally with:
- Email: `alvarnat@sheridancollege.ca`
- Name: `Natasha Alvarado Dubkova`

NatashaAlv: delete section id intro and the footer

GitHub Copilot: Read [](file:///Users/sinnacado/Desktop/Project-2/public/index.html)

Using "Replace String in File"


```

```
Done! The `#intro` section and footer have been removed from the HTML.

Made changes.

NatashaAlv: change the color scheme to a dark theme with cool tones

GitHub Copilot: Using "Multi-Replace String in Files"


```

```
Done! The color scheme has been updated to a dark theme with cool tones:
- Background: Dark blue-gray (#1a2332)
- Cards and forms: Cool dark slate (#2a3647)
- Borders: Medium cool gray (#3d4f66)
- Text: Light blue-gray (#e0e6ed)
- Accent buttons: Cool blue (#2d7a9e)
- Meters and inputs: Cool blue tones
- Delete button: Muted cool red/purple

Made changes.

NatashaAlv: add endTime String under startTime String in schema.prisma

GitHub Copilot: Read [](file:///Users/sinnacado/Desktop/Project-2/prisma/schema.prisma#1-1), lines 1 to 20

Using "Replace String in File"


```

```
Done! Added `endTime String` field after `startTime` in the schema.

Made changes.

NatashaAlv: add endTime to index.html script.js and style.css in the same way as startTime

GitHub Copilot: Using "Multi-Replace String in Files"


```

```

```

```
Done! Added `endTime` field to:
- HTML form with the same styling as `startTime`
- JavaScript rendering to display the end time alongside start time in the session cards

The CSS styling will automatically apply since the endTime uses the same `.stat` class as startTime.

Made changes.

NatashaAlv: Change Subject Type into a drop down with options, like art, science, math

GitHub Copilot: Read [](file:///Users/sinnacado/Desktop/Project-2/public/index.html#75-75), lines 75 to 95

Using "Replace String in File"


```

```
Done! Changed Subject Type from a text input to a dropdown select with options: Art, Science, Math, English, History, Computer Science, and Other.

Made changes.

NatashaAlv: Change Productive Time and Distracted Time into sliders that have a minimum of 0% and a maximum of 100%

GitHub Copilot: Read [](file:///Users/sinnacado/Desktop/Project-2/public/index.html#140-140), lines 140 to 170

Read [](file:///Users/sinnacado/Desktop/Project-2/public/index.html#165-165), lines 165 to 180

Using "Multi-Replace String in Files"


```

```

```

```
Done! Changed Productive Time and Distracted Time to range sliders with:
- Minimum: 0%
- Maximum: 100%
- Default value: 50%
- Display updated to show percentages instead of hours

Made changes.

NatashaAlv: Add a "0" text to the left of both sliders and a "100" text to the right of both sliders. Underneath both sliders show the active percentage in relation to the positioning of the sliders.

GitHub Copilot: Read [](file:///Users/sinnacado/Desktop/Project-2/public/index.html#148-148), lines 148 to 180

Using "Multi-Replace String in Files"


```

```


Using "Replace String in File"


```

```


Using "Replace String in File"


```

```
Done! Added:
- "0" label on the left and "100" label on the right of both sliders
- Live percentage display underneath each slider that updates as you move the slider
- JavaScript to handle real-time updates and form reset
- CSS styling for the slider containers and value displays

Made changes.

NatashaAlv: add a slight drop shadow effect to #createButton

GitHub Copilot: Read [](file:///Users/sinnacado/Desktop/Project-2/public/style.css#120-120), lines 120 to 140

Using "Replace String in File"


```

```
Done! Added a subtle drop shadow effect to the create button.

Made changes.
