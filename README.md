# Music Generation of Jazz Style based on Deep Learning 

 This paper studies the music generation, and constructs a jazz style music generation model and interactive platform based on deep learning. 

***

## ABSTRACT

With the rapid development of deep learning technology, researchers are also applying computer technology to art generation. Many neural network models have also performed well in music generation. However, existing music generation projects generally have the following problems: 1. There is little correlation between the sections of music generated, and the overall structure is relatively random. 2. Most models are used to learn and produce classical or popular music. 3. The final output cannot be manually controlled, and there is little interaction between the model and the user.
In order to solve the above problems, based on previous studies, this paper studies the music generation, and constructs a jazz style music generation model and interactive platform based on deep learning. The main research contents are as follows:
1. Lakh MIDI data set was used to match the metadata information in the Million Song data set, and then jazz music was screened by API. Finally, the percussion and piano tracks are separated and the jazz music data sets of the two instruments are constructed.
2. Based on the LSTM network model of Google's Magenta open source library, two kinds of music generation models are established: a percussion model that can generate drumbeats and a piano model that can generate melodies. One-hot coding was used for the input sequence of notes, and the backtracking mechanism and attention mechanism were used to enable the model to learn the music structure in the bar.
3. The model is trained with data sets. The trained model is used to read the input sequence of notes, generate the jazz percussion and piano melody according to the input, and objectively and subjectively evaluate the generated results.
4. Finally, the model is implemented in a Web browser. Users can input the initial sequence of notes in the browser, use the model to generate music, and process the music to some extent. So as to achieve the purpose of human-computer interaction.

***

# Model

## Database

If you want to use our database, can be in <https://pan.baidu.com/s/184t4GPW_-qhjeGF8TYcFKg> (extraction code: uj3i) to download.


The __training__ folder is a trained model where you can use the bundled files to generate music from the command line.

If you would like to hear the partial results generated please go to <https://github.com/AmintaCXY/Result/tree/master> .

***

# Web


You can view the [demo video](https://www.iqiyi.com/v_19rxoxegck.html#curid=16679132200_31e68db468b23d137405e651ce48e8cb) before using it.


In the __web__ folder is the web source file for music generation interaction. 
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
