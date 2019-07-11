Back to [Projects List](../../README.md#ProjectsList)

## Image Quizzer Project

## Key Investigators
- Carol Johnson (Baines Imaging Research Laboratory, London Regional Cancer Program) 

# Project Description
<!-- Add a short paragraph describing the project. --> 
The goal of the Image Quizzer project is to develop a clinical tool that can be used for educational purposes.
Upon presenting patient images to a user, the user is required to answer some customized questions.
Having this tool integrated in Slicer, the user can make use of the existing image viewing functionality.
The user's responses to the quiz are captured for offline analysis.

## Objective
- To create a slicelet that will present to the user a series of images with an associated questionnaire. 
- An administrator will be able to dynamically customize the questionnaire to suit the teaching application. 
- User responses to the questionnaire will be captured for analysis.

## Approach and Plan
- Image Quizzer Designer application
    - Using Qt Designer and python, create application to allow an administrator to design a quiz.
    - The administrator will be able to add group boxes which will hold questionnaire items (radio buttons, toggle switch, line edit boxes etc.)
    - The designed quiz must be captured into a ui file which is ported to the Image Quizzer application.
- Image Quizzer Study Browser
    - An application that defines which patients and their associated series are going to be presented with the questionnaire.
    - Develop a method to display to the users which patients have been processed (completed or partially completed) in Image Quizzer and which patients are outstanding.
- Image Quizzer application
    - Create a slicelet to load customized quiz from ui file.
    - Display images in a controlled fashion allowing for 'next' and 'back' button options.
    - Capture quiz responses in xml format once user presses 'save'.

## Progress and Next Steps

<!--Describe progress and next steps in a few bullet points as you are making progress.-->
- Image Quizzer Designer
  - A skeleton program has been created for the Image Quizzer Designer that can dynamically add a group box along with customized questionnaire items.
  - The customized quiz can be previewed.
  - TODO: 
      - Flesh out python code to dynamically create the widgets - providing the user with more design tools
      - Learn how to capture/save the dynamically created QWidget and it's contents in a .ui file.
- Image Quizzer Study Browser
  - TODO:
      - Learn how to work with Slicer's data base module to create the list of patients and their images for the quiz.
      - Learn how to coordinate a study progress tool.
- Image Quizzer
  - A skeleton slicelet program has been developed to load a .ui file to present the customized quiz. 
  - The quiz is shown beside patient images.
  - TODO:
      - Learn how to capture the user responses to the quiz.
      - Learn how to coordinate Next and Back buttons based on the patient images and their series organized by the Study Browser tool.
         

# Illustrations

<!--Add pictures and links to videos that demonstrate what has been accomplished.-->

<!--![Description of picture](Example2.jpg)-->

<!--![Some more images](Example2.jpg)-->

# Background and References

<!--Use this space for information that may help people better understand your project, like links to papers, source code, or data.-->
- Reference to an observer study that was developed by our lab using the ClearCanvas Workstation
    - Mattonen SA, Palma DA, Johnson C, Louie AV, Landis M, Rodrigues G, Chan I, Etemad-Rezai R, Yeung TPC, Senan S, Ward AD, Detection of local cancer recurrence after stereotactic ablative radiotherapy (SABR) for lung cancer: physician performance versus radiomic assessment, International Journal of Radiation Oncology • Biology • Physics (2016), doi: 10.1016/j.ijrobp.2015.12.369.




