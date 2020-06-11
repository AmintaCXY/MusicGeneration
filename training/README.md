# Model

 This is a trained model where you can generate music in the following ways:

 Start by creating a new environment:
 
    conda info
    conda create --name magenta python=3.6`

 Activate the environment we created and install the library in it:
 
    conda activate magenta
    pip install magenta==1.1.7

 Then use the following code to generate music using the model, replace `bundle` with the mag file address, and replace `output` with the output directory:
 
    drums_rnn_generate --bundle_file="bundle" --output_dir="output"

 `primer` can be replaced with the input MIDI file address:：
 
    melody_rnn_generate --bundle_file="bundle" --output_dir="output"  --primer_midi="primer"
     
