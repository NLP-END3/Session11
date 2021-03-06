# Session 11 (task3)
The School of AI - END3 Course, Session 11 Assignment Task 3

*Group Members: Dhruba Adhikary, Phani Nandula, Prateek Maheshwari, Sujit Ojha*

# Assignment
These are the assignments that you'd be doing this and next week!

- **TASK 3 (Week 2)**: Reproduce the training explained in this blog. You can decide to pick fewer datasets.
- **Proceed to Session 11** - Assignment Solutions page and:
    - Submit README link for Task 3 (training log snippets and 5 sample results along with BART description must be available) - 1000 points

# Input Text Dataset:
Due to memory constarins faced while running in the Colab we have chosen only Google Data to finetune the BART model.
Some of the changes made to the code to over come the memory issues are:   
1. Reducing the training dataset size from 3 datasources (Google dataset, MSRP dataset from Microsoft, Quora dataset) to 1 dataset (Google Dataset)
2. Reduce the number of training batch size from 8 to 4 (***model_args.train_batch_size = 4 #8***)
3. Reduce the number of eval batch size from 64 to 8 (***model_args.eval_batch_size = 8 #64***)
4. Included the ***model_args.fp16 = True***
# Notebook
- [Link](BART_paraphrasing.ipynb) 

# Training Logs
![TrainingLogs](https://user-images.githubusercontent.com/30425824/151531581-8505725e-f50b-4ae6-aa8d-e1c0b1ae9a5b.png))

# Sample Results
![Example1 & 2](https://user-images.githubusercontent.com/30425824/151531763-f5a7fc0f-6386-4f24-b97a-ae33f69e6072.png)
![Example3 & 4](https://user-images.githubusercontent.com/30425824/151531857-73f10618-56f8-47bf-8afb-8b4b5fbf1a7b.png)
![Example5 & 6](https://user-images.githubusercontent.com/30425824/151531983-84523cb7-fc62-4f5f-8495-374bcb3b2363.png)
![Example6 & 7](https://user-images.githubusercontent.com/30425824/151532179-c187d6e9-e6a5-479a-9810-90bc8328c6b8.png)
