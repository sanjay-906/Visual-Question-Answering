## Visual-Question-Answering

- VQA involves training ml model which can answer questions based on a given image
- Implemented using Text and Vision transformers

## Dataset
![daquar-dataset](https://github.com/sanjay-906/Visual-Question-Answering/assets/99668976/8c9171a2-5333-48f5-9477-4a3476a1d9ed)

- DAQUAR (DAtaset for QUestion Answering on Real-world images) is a dataset of human question answer pairs about images

## Model Architecture
![arch](https://github.com/sanjay-906/Visual-Question-Answering/assets/99668976/ff494cc8-ca9c-4f5e-80ec-b33b42a67c7a)

- The outputs of both the transformers are merged in a fully connected layer

## Predictions
![predictions](https://github.com/sanjay-906/Visual-Question-Answering/assets/99668976/38121ba3-f94b-4b7f-b0e7-48a63bdea5ce)


## Results
| Metric           | Standard    | QLoRA       | Change    | Effect    |
|------------------|-------------|-------------|-----------|-----------|
| WUPS             | 0.264536    | 0.246825    | -6.695%   | 🔴       |
| Accuracy         | 0.212510    | 0.190457    | -10.377%  | 🔴       |
| F1-score         | 0.016420    | 0.011313    | -31.10%   | 🔴       |
| Time complexity  | 88.462s     | 104.051s    | +17.622%  | 🔴       |
| Space complexity | 7,78,448 KB | 2,05,483 KB | -73.603%  | 🟢       |
| No of parameters | 199238631   | 115188711   | -42.185%  | 🟢       |

### No of parameters:

|                   | Total params | Trainable params | Trainable % | Effect |
|-------------------|----------------------|----------------|-------------------|--------|
| Standard   | 199238631            | 199238631      | 100.0% | 🔴 |
| QLoRA             | 115188711              |   4251879     | 3.691% | 🟢 |

## Training results
![vqa_graphs_page-0001](https://github.com/user-attachments/assets/a7857bd6-70ec-4a84-bf1f-362cb877aa87)


## Try Out
OUTPUT: <a href="https://huggingface.co/spaces/sanjay-906/VQA" target="_blank">Click Here</a>

