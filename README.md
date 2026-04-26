Aidan Akenson

===================== METHOD =====================  
I broke the task down into components I could  
tackle more easily individually and then chain   
together.  

1. I used the pseudocode you provided to make a   
frequency power checking function. This was tested  
against a continuous 2025 Hz tone and a continuous   
2225 Hz tone.  

2. I created a function that checks the correlation  
between the mark (2225 Hz) and space (2025 Hz) tones  
for each bit in a byte. This was tested on the above  
signals, as well as a signal that alternated which  
frequency it contained every bit.  

3. I made a simple byte-to-ascii converter.  

4. I wrote a decode function which simply takes the  
data from a .wav file and processes every data bit  
while ignoring the start and stop bits. The ascii  
conversion is then run, and a string is generated  
and printed representing the contents of the file.  


===================== SETUP =====================  
Make sure Jupyter Notebook, numpy, and soundfile  
are installed, then run modem.ipynb.  
