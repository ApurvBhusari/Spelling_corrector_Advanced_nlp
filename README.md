# Spelling_corrector_Advanced_nlp
### Problem Statement
Spelling correction in natural language processing and information retrieval literature mostly relies on pre-defined lexicons to detect spelling errors. Spelling correction is the task of detecting and correcting spelling mistakes.

### Solution Proposed: BERT-Based Spelling Corrector

#### Overview:
The proposed solution aims to leverage the power of BERT (Bidirectional Encoder Representations from Transformers) for spelling correction in natural language processing and information retrieval tasks. Instead of relying solely on pre-defined lexicons, we'll harness the contextual understanding capabilities of BERT to detect and correct spelling mistakes.

#### Steps:

1. **Data Preparation**:
   - Collect a large corpus of text data that includes both correctly spelled and misspelled words. This corpus will be used to train and fine-tune the BERT model for spelling correction.

2. **Preprocessing**:
   - Tokenize the text data into input sequences suitable for BERT.

3. **Fine-tuning BERT**:
   - Fine-tune a pre-trained BERT model on the misspelled and correctly spelled word pairs. This fine-tuning process helps the model learn contextual patterns related to spelling mistakes.

4. **Model Architecture**:
   - Utilize a BERT-based architecture, potentially using a modification of the BERT model specifically designed for spelling correction (e.g., SpellBERT).

5. **Inference**:
   - When a piece of text is input into the model, it processes the entire sequence in a bidirectional manner, allowing it to understand the context in which each word is used.

6. **Spelling Correction**:
   - Identify candidate misspelled words by comparing them to a dictionary or a pre-defined lexicon. These candidates will be passed through the BERT-based spelling corrector.

7. **Contextual Correction**:
   - The BERT-based model considers the surrounding context of each word to determine the most likely corrected form. This context-awareness is a key advantage of using BERT for spelling correction.

8. **Output**:
   - The model produces corrected versions of the misspelled words, which are then integrated back into the original text.

#### Benefits:

- Context-Aware Corrections: BERT's bidirectional processing allows it to understand the context in which words are used, leading to more accurate and contextually appropriate corrections.
- Reduced Reliance on Lexicons: While pre-defined lexicons are still useful, the model's contextual understanding helps identify and correct spelling mistakes that may not be present in the lexicon.
- Improved Accuracy: The fine-tuning process helps tailor the model specifically for spelling correction, potentially leading to higher accuracy compared to generic models.

#### Considerations:

- Model Training Data: The quality and diversity of the training data for fine-tuning the BERT model are crucial for its effectiveness.
- Evaluation Metrics: Establish metrics to evaluate the performance of the spelling correction model, potentially using validation sets with known misspellings.

This proposed solution leverages BERT's contextual understanding to enhance spelling correction capabilities, potentially offering a more robust and accurate approach compared to traditional lexicon-based methods.


## Tech Stack Used
1. Python 
2. Flask
3. Tensorflow(keras)
4. Docker
5. MongoDB

## Infrastructure Required.

1. AWS S3
2. AWS EC2
3. AWS ECR
4. Git Actions
5. Terraform

## How to run?
Before we run the project, make sure that you are having MongoDB in your local system, with Compass since we are using MongoDB for data storage. You also need AWS account to access the service like S3, ECR and EC2 instances.


## Deployment Archietecture
![image](https://user-images.githubusercontent.com/57321948/193536973-4530fe7d-5509-4609-bfd2-cd702fc82423.png)



### Step 1 - Install the requirements

```bash
pip install -r requirements.txt
```

### Step 2 - Run main.py file

```bash
python main.py
```

To download your dataset

```
wget https://raw.githubusercontent.com/avnyadav/sensor-fault-detection/main/aps_failure_training_set1.csv
```

This is changes made in neuro lab

Git commands

If you are starting a project and you want to use git in your project
```
git init
```
Note: This is going to initalize git in your source code.


OR

You can clone exiting github repo
```
git clone <github_url>
```
Note: Clone/ Downlaod github  repo in your system


Add your changes made in file to git stagging are
```
git add file_name
```
Note: You can given file_name to add specific file or use "." to add everything to staging are


Create commits
```
git commit -m "message"
```

```
git push origin main
```
Note: origin--> contains url to your github repo
main--> is your branch name 

To push your changes forcefully.
```
git push origin main -f
```


To pull  changes from github repo
```
git pull origin main
```
Note: origin--> contains url to your github repo
main--> is your branch name


.env file has
```
MONGO_DB_URL="mongodb://localhost:27017"
AWS_ACCESS_KEY_ID="aagswdiquyawvdiu"
AWS_SECRET_ACCESS_KEY="sadoiuabnswodihabosdbn"
```

```
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo usermod -aG docker ubuntu
newgrp docker
```


```


AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=
AWS_ECR_LOGIN_URI=
ECR_REPOSITORY_NAME=
BUCKET_NAME=
MONGO_DB_URL=
```























