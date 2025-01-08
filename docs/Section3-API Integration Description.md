# API Integration Description

### Endpoint
`POST /ogccdrp24.focusit.com.tw/ask`

### Description
This endpoint allows users to ask questions based on `specific data or knowledge they want to inquire about.`

### Request Body
The request body should be a JSON object with the following structure:
```
{
  "question": "string"
}
```
| Method      | Type        | Required    | Description     |
| ----------- | ----------- | ----------- | --------------- |
| question    | string      | yes         | The "question" parameter represents the inquiry or query to be made. It should contain the specific question the user wants to ask. |

### Response
The response will be a JSON object with the following structure:
```
{
  "answer": "string"
}
```

The data array will contain the matching result based on the provided search criteria. The item in the array will have the following properties:

| Method      | Type        | Description     |
| ----------- | ----------- | --------------- |
| answer      | string      | The result of the question. |

!!! info "Response Mechanism Explanation"
    The response will first be classified by the AI to determine the type of question. Based on the identified type, the corresponding vector database will be queried to generate an appropriate answer. Therefore, please provide detailed questions to ensure accurate responses.
    
    If you want to know the available keywords, please click [here](http://127.0.0.1:8000/ogc-demo-web/Section2-Data%20Processing%20Method/).

### Example of Usage
To ask for climate change increase the risk of flooding in Canada.
```
{
  "question": "How does climate change increase the risk of flooding in Canada?"
}
```
#### Output:
```
{
  "answer": "Climate change increases the risk of flooding in Canada by causing more intense and frequent rainfall events, leading to increased flood risk in urban areas. Additionally, the loss of sea ice from a warming climate contributes to higher storm surges and waves, particularly in Atlantic Canada. Snowmelt runoff floods, which are common in Canada, occur due to rapid melting of snow under warmer temperatures, resulting in heavy runoff when the ground is frozen."
}
```