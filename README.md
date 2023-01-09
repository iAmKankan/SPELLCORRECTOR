# SPELLING CORRECTOR

## DESCRIPTION OVERVIEW
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

A word needs to be checked for spelling correctness and corrected if necessary, many a time in the context of the surrounding words. A spellchecker points to spelling errors and possibly suggests alternatives. An autocorrector usually goes a step further and automatically picks the most likely word. In case of the correct word already having been typed, the same is retained.

There are different types of spelling errors.

1. **Non-word Errors:** These are the most common type of errors. You either miss a few keystrokes or let your fingers hurtle a bit longer. E.g., typing langage when you meant language; or hurryu when you meant hurry

2. **Real Word Errors:** If you have fat fingers, sometimes instead of creating a non-word, you end up creating a real word, but one you didn’t intend. E.g, typing buckled when you meant bucked. Or your fingers are a tad wonky, and you type in three when you meant there.

3. **Cognitive Errors:** The previous two types of errors result not from ignorance of a word or its correct spelling. Cognitive errors can occur due to those factors. The words piece and peace are homophones (sound the same). So you are not sure which one is which. Sometimes your damn sure about your spellings despite a few grammar nazis claim you’re not.

4. **Short forms/Slang/Lingo:** These are possibly not even spelling errors. May be u r just being kewl. Or you are trying hard to fit in everything within a text message or a tweet and must commit a spelling sin. We mention them here for the sake of completeness.


## TECHNOLOGY USE
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

Here we will be using  Anaconda Python 3.6 , Keras 2.2.4 using TensorFlow GPU 1.14.0 backend CUDA 10 with CuDNN 10 

## INSTALLATION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Installation of this project is pretty easy. Please do follow the following steps to create a virtual environment and then install the necessary packages in the following environment.

**In Pycharm it’s easy** 

1. Create a new project.
2. Navigate to the directory of the project
3. Select the option to create a new new virtual environment using conda with python3.6
4. Finally create the project using used resources.
5. After the project has been created, install the necessary packages from **requirements.txt** file using the command _`pip install -r requirements.txt`_


**In Conda also it’s easy**

1. Create a new virtual environment using the command
    _`conda create -n your_env_name python=3.6`_
2. Navigate to the project directory.
3. Install the necessary packages from requirements.txt file using the command _`pip install -r requirements.txt`_



## WORKFLOW DIAGRAM
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211360421-488f9397-4ade-4efa-9fee-1f97e5ce9c26.png" width=60%/>
</p>


## IMPLEMENTATION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

### 1. Project Directory 
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211360559-46998a1e-563d-4721-93cd-2f3d62edc1f0.png" width=60%/>
</p>

This above picture is of the project directory if we open the project folder using Pycharm. In the directory different types of files are there like for speliingcorrector, flask server etc. 

### 2. requirements.txt
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)


<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211360745-9e3f1599-3224-4926-ac25-51bd3ca564ac.png" width=60%/>
</p>

This file consists of the sequence to squence model architecture that has been built using Keras framework. 

### 3. spellingcorrector.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)


<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211360891-271b71e8-c6a6-464c-b2b0-afe9578e631a.png" width=60%/>
</p>


This file consists of the prediction process.


### 4. clientApp.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)


<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211361085-1fc5af2d-8e38-4feb-857f-f27a76a2a037.png" width=60%/>
</p>

This file consists of flask and this is the entry point of application.

## TESTING IN LOCAL/API
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

To do the test testing we need to run the **clientApp.py** and after that web server will start at **http://0.0.0.0:5000/**

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211362014-cc10114d-2a3e-4e27-b764-ed6ac8b8dd46.png" width=60%/>
</p>

Enter the wrong spelled sentence and click on predict.
 
<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211361898-8b50bce5-feb6-4d62-9ff6-1c6735f9037c.png" width=60%/>
</p>

After clicking Predict


<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211361800-862a5222-ce06-46cf-84e6-21984d8860b6.png" width=60%/>
</p>

Finally the answers are shown in the results box.

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211361718-27a74d3d-a801-4900-b42e-7e8a8d9e8be1.png" width=60%/>
</p>

## CONCLUSION	
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

Here we have successfully built a spelling checker and corrector which can be used to correct spelling if the user gives misspelled words.

## COMPARISION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

We can build better accurate models using pretrained models like BERT, GPT2 etc. Also here we have given very less training data but the user can increase the sizing of training data which will help to build a better model with better prediction.
