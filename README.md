## Step to run MCQGEN
- Clone mcqgen in your local machine
- Download and install Anaconda from https://www.anaconda.com/download
- Type anaconda on windows search and open anaconda command prompt
- Navigate to mcqgen progect (in step 1) from conda prompt and/by follow below commands
    * cd <basepath>/mcqgen
    * conda create -p env python=3.8 -y
    * pip install -r requirement.txt
    * python setup.py install
- Create a file with name '.env' in mcqgen folder
- Add below line in .env file
    * OPENAI_API_KEY="Supply your secret token here"
- Open StreamlitAPP.py (notepad++ or VS Code) and configure Response.json file path at line number 11 with appropriate value 
- Run mcqgen with below command
    * streamlit run StreamlitAPP.py --server.port 8080