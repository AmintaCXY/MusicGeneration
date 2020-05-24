# Music Generation of Jazz Style based on Deep Learning 

 This paper studies the music generation, and constructs a jazz style music generation model and interactive platform based on deep learning. 


***

The __training__ folder is a trained model where you can use the bundled files to generate music from the command line.

If you would like to hear the partial results generated please go to <https://github.com/AmintaCXY/Result/tree/master> .

***

In the __web__ folder is the web source file for music generation interaction. 
You can download this folder and use __start.py__ to start the server locally. 

The default file placement path is `/Downloads/MusicGeneration-master`. 
Modify this path if you are placing the file in a different location, but at the same time you need to modify the __checkpoints__ path under __script.py__  file.

## Mac:

    python ./Downloads/MusicGeneration-master/web/start.py 8000

## Windows:

    python .\Downloads\MusicGeneration-master\web\start.py 8000

Then you can open the __musicgeneration.html__ page under the __web__ file.

The page is then used to generate music.
