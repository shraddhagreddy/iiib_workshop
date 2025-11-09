# Things covered today
- prompting
- evaluate and iterate framework
- chatgpt
- Api keys - gemini
- try to create chatbot 
- LANG Flow based - no coding tools
- spin off projects
- MCP, RAG, Agentic

### burt, bath models

## Langflow
- similar to n8n 
- n8n is a more business end of things
- Langflow is more engineering end of things

## Google AI STudio
- so when we use Gemini 2.5 Flash Lite which was updated in jan2025 without enabling grounding with google search
- it gives president of USA is Joe Biden
- but after enabling the grounding w google search then it gives the correct president 
- earlier, CHATGPT 4 and all it had a drawback of hallucination
- product poisitioning has improved since then
- Gemini 2.5 pro (March 2025) -> doesnt know about its existence- so when we try to generate ur application it generates with Gemini 1.5
- this is due to the lack of context
- API brings the model, chassis is ur duty for context
- 0 shot prompting

## What is chatgpt?
- when we search for who is the president of USA without enabling web search
- still gives correct answer
- its a product- checked if it should go to the web or not
- chose to search the web
- eventhough u gave a 0 shot prompting
- it realised that it requires more context
- github copilot is also a sw tool 


# one shot prompting

## Task 1
- create a face detection application
- context:
    - use python language
    - create conda environment iitb_face_detect_evn with python 3.10
    - use opencv library and haarclassifier from that library
    - use 'q'to quit
    - draw Green coloured bounding boxes over the faces detected
    - provide the count of number of faces on the top left
- arch:
    - face_det.py
    - requirements.txt
    - readme.md

## prompt2:

- here from the image button1 will be for the start/stop the video stream
- button2 will be for capturing the image
- save the captured image into a folder called collections


## prompt 3:
- i want the ui to be separated out.
- use tkinter for gui
- ensure on opening the size of the window is about half the size of my desktop height and width

- architecture:
    - face_det.py: houses code only for face detection
    - ui.py: the ui related code
    readme.md: defining the details of the project
    collections: folder for captured images
    -- img_hhmmss_ddmmyy.png


- Task 
- Context 
- Reference 
- Evaluate 
- Iterate


## chatgpt
- i want to build an application to draw on the screen where i will use my fingers
- 
- - create a face detection application
- context:
    - use python language
    - create conda environment iitb_face_detect_evn with python 3.10
    - use opencv library and haarclassifier from that library
    - use 'q'to quit
    - draw Green coloured bounding boxes over the faces detected
    - provide the count of number of faces on the top left
- arch:
    - face_det.py
    - requirements.txt
    - readme.md
- use tkinter for gui
- ensure on opening the size of the window is about half the size of my desktop height and width

- architecture:
    - face_det.py: houses code only for face detection
    - ui.py: the ui related code
    readme.md: defining the details of the project
    collections: folder for captured images
    -- img_hhmmss_ddmmyy.png