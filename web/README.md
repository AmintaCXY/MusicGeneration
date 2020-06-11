# Web


You can view the [demo video](https://www.iqiyi.com/v_19rxoxegck.html#curid=16679132200_31e68db468b23d137405e651ce48e8cb) before using it.

You can download this folder and use __start.py__ to start the server locally. 

The default file placement path is `/Downloads/MusicGeneration-master`. 
Modify this path if you are placing the file in a different location, but at the same time you need to modify the __checkpoints__ path under __script.py__  file.

## Mac

    python ./Downloads/MusicGeneration-master/web/start.py 8000

## Windows

    python .\Downloads\MusicGeneration-master\web\start.py 8000

Then you can open the __musicgeneration.html__ page under the __web__ file.

The page is then used to generate music.

It is important to note that the notes are entered from the __left__ side of the panel so that the model can generate subsequent music.
