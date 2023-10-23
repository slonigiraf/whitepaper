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
| 0  | List  | {"t" : 0, "h" : "USA school curriculum", "e": [...]} |
| 1  | Course  | {"t" : 1, "h" : "Math for 5th grade", "e": [...]} |
| 2  | Module  | {"t" : 2, "h" : "Working with fractions", "e": [...]} |
| 3  | Skill  | {"t" : 3, "h" : "Adding two fractions", "e": [...]} |
| 4  | Exercise  | {"t" : 4, "q" : {"h" : "What is a result of 1/3+1/3?", f: "answer optional file id"}, "a" : {"h": "2/3", f: "answer optional file id"}} |
