<p align="center"><h1>🤖 Getting Started</h2></p>
<p align="left"><h3>⭐️Jupyter Lab Guide</h3></p>

1.	Install Jupyter lab or Jupyter lab cloud  
        •	 https://jupyter-batch-us-region-1.cloud.intel.com/user/u37b6cfaa417403454509c45c11d2628/lab/tree/Training/AI/GenAI<br>
 	     •	 https://jupyter.org/install
       
2.	Start the server


---

<p align="left"><h3>⭐️Requirements</h3></p>
1.	Stable Internet connection <br>
2.	Memory and disk space required per user: 512MB RAM + 1GB of disk + .5 CPU core.<br>
3.	Server overhead: 2-4GB or 10% system overhead (whatever is larger), .5 CPU cores, 10GB disk space.<br>

<p align="left"><h3>⭐️Required Packages</h3></p>
1.	intel-extension-for-transformers <br> <p align = "left">https://github.com/intel/intel-extension-for-transformers</p>
2.	llama-2-7-hf-b model <br><p align ="left">https://huggingface.co/meta-llama/Llama-2-7b-chat-hf</p> 
3.	Huggingface id with access token permissions "Fine grained & Write permission" <p align ="left">https://huggingface.co/</p>

<p align="left"><h3>⭐️Step by step procedure to run the notebooks</h3></p>
  <h3>Terminal :</h3> <br>
   1.Create an anaconda environment:

```
       $conda create -n itrex python=3.10 -y
```
  2.Activate the environment:
```
       $conda active itrex
```
  3.Install the pip package of requirements 
```
       $pip install intel-extension-for-transformers
```
  4.Clone the following repository
```
       $git clone https://github.com/intel/intel-extension-for-transformers.git
```
  5.Install the pip package of CPU requirements
```
       $pip install -r requirements_cpu.txt
```
  6.Login with the huggingface id with a newly created access token
```
       $huggingface-cli login
```            
  7.Install the kernel for the environment
```
       $python3 -m pip install jupyter ipykernel
```
  8.Create the kernel with user permission 
```
       $python3 -m ipykernel install –name neural-chat --user
```
 
•	First Notebook :  build_chatbot_on_spr.ipynb
1.	Select the kernel we created “neural_chat”
2.	Run all the cells and you will get an output
 
 
 

•	Second Notebook : single_node_finetuning_on_spr.ipynb
Terminal :
1.	Import llama model
2.	Create an access token with permission write
3.	Login with huggingface with newly created token 
4.	Import alpaca dataset
5.	In notebook Run all the cells and record training time

 


•	Third Notebook :  single_node_finetuning_on_spr.ipynb  on google collab 
1.	Import the notebook into google collab 
2.	Run all the cells by selecting runtime type to CPU 
3.	Record training time 

 

              
