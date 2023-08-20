# Data format for giraf module
## JSON types

| Id | Description | Example |
| -- | ----------- | ------- |
| 0  | Basic list  | {"s" : 0, "h" : "Example header", "e": [...]} |
| 1  | List of courses  | {"s" : 1, "h" : "USA school curriculum", "e": [...]} |
| 2  | List of modules  | {"s" : 2, "h" : "Math for 5th grade", "e": [...]} |
| 3  | List of skills  | {"s" : 3, "h" : "Working with fractions", "e": [...]} |
| 4  | Skill  | {"s" : 4, "h" : "Adding two fractions", "e": [...]} |
| 5  | Task for skill training  | {"s" : 5, "q" : {"h" : "What is a result of 1/3+1/3?", f: "answer optional file id"}, "a" : {"h": "2/3", f: "answer optional file id"}} |
