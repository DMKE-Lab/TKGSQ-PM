# TKGSQ-PM

Temporal Knowledge Graph Semantic Query based on Pre-trained Model

# Installation

Torch1.7.1+cu110
numpy
pickle
collections
scikit-learn
transformers
tqdm

install the TKGSQ-PM requirements:

conda install requirements.txt -c conda-forge


# Usage

(Take dataset MultiTQ as an example,the operation of other data sets is similar to the command.)
information recognize part:

cd TKGSQ-PM
python ner_task.py

# train and test:

We use TComplEx KG Embeddings as implemented in https://github.com/facebookresearch/tkbc.

python train_qa_model.py --dataset MultiTQ --model TKGSQ_PM  --max_epoch 20 --learning_rate 2e-4 --batch_size 100 –save_to MultiTQ.log
