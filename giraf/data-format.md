# Data format for giraf module
## JSON types

| Key | Description | Example |
| --- | ----------- | ------- |
| t | type, numeric | "0" |
| h | header, text | "Math, 5th grade" |
| p | parents, list of parent ids | ["0x3c183aa5c72de3df5eef266849171413d761d3c798b780639e71c3d0ef589701", "0xf55ff16f66f43360266b95db6f8fec01d76031054306ae4a4b380598f6cfd114", "0x3292a9e0163fc54de85e099c931132b05bf5e30d00fc5e99c8d5e2df95c08b07"] |
| q | question, text | "How much is a 2+2?" |
| a | answer, text | "2+2 is 4" |

| Id | Description | Example |
| -- | ----------- | ------- |
| 0  | Basic list  | {"t" : 0, "h" : "Example header", "e": [...]} |
| 1  | List of courses  | {"t" : 1, "h" : "USA school curriculum", "e": [...]} |
| 2  | List of modules  | {"t" : 2, "h" : "Math for 5th grade", "e": [...]} |
| 3  | List of skills  | {"t" : 3, "h" : "Working with fractions", "e": [...]} |
| 4  | Skill  | {"t" : 4, "h" : "Adding two fractions", "e": [...]} |
| 5  | Task for skill training  | {"t" : 5, "q" : {"h" : "What is a result of 1/3+1/3?", f: "answer optional file id"}, "a" : {"h": "2/3", f: "answer optional file id"}} |
