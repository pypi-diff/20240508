# Comparing `tmp/PyTorch-Beacon-0.0.7.tar.gz` & `tmp/pytorch_beacon-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTorch-Beacon-0.0.7.tar", last modified: Sat Oct 28 22:06:34 2023, max compression
+gzip compressed data, was "pytorch_beacon-0.1.0.tar", last modified: Wed May  8 18:17:34 2024, max compression
```

## Comparing `PyTorch-Beacon-0.0.7.tar` & `pytorch_beacon-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-10-28 22:06:34.920250 PyTorch-Beacon-0.0.7/
--rw-rw-rw-   0        0        0     1050 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.7/LICENCE
--rw-rw-rw-   0        0        0      532 2023-10-28 22:06:34.917688 PyTorch-Beacon-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-10-28 22:06:34.823507 PyTorch-Beacon-0.0.7/PyTorch_Beacon.egg-info/
--rw-rw-rw-   0        0        0      532 2023-10-28 22:06:34.000000 PyTorch-Beacon-0.0.7/PyTorch_Beacon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-10-28 22:06:34.000000 PyTorch-Beacon-0.0.7/PyTorch_Beacon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-28 22:06:34.000000 PyTorch-Beacon-0.0.7/PyTorch_Beacon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-10-28 22:06:34.000000 PyTorch-Beacon-0.0.7/PyTorch_Beacon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      208 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-10-28 22:06:34.907499 PyTorch-Beacon-0.0.7/beacon/
--rw-rw-rw-   0        0        0      122 2023-07-22 18:00:51.000000 PyTorch-Beacon-0.0.7/beacon/__init__.py
--rw-rw-rw-   0        0        0     7778 2023-10-28 21:36:08.000000 PyTorch-Beacon-0.0.7/beacon/dataloading.py
--rw-rw-rw-   0        0        0      972 2023-10-28 16:48:14.000000 PyTorch-Beacon-0.0.7/beacon/metrics.py
--rw-rw-rw-   0        0        0     7130 2023-10-28 16:48:14.000000 PyTorch-Beacon-0.0.7/beacon/module.py
--rw-rw-rw-   0        0        0     4232 2023-10-28 16:48:14.000000 PyTorch-Beacon-0.0.7/beacon/training.py
--rw-rw-rw-   0        0        0     2551 2023-07-19 17:13:10.000000 PyTorch-Beacon-0.0.7/beacon/utils.py
--rw-rw-rw-   0        0        0      480 2023-10-28 22:04:15.000000 PyTorch-Beacon-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-28 22:06:34.920250 PyTorch-Beacon-0.0.7/setup.cfg
+drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2024-05-08 18:17:34.953505 pytorch_beacon-0.1.0/
+-rw-r--r--   0 lukelele   (501) staff       (20)     1050 2023-07-17 15:38:51.000000 pytorch_beacon-0.1.0/LICENCE
+-rw-r--r--   0 lukelele   (501) staff       (20)      613 2024-05-08 18:17:34.953170 pytorch_beacon-0.1.0/PKG-INFO
+drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2024-05-08 18:17:34.952764 pytorch_beacon-0.1.0/PyTorch_Beacon.egg-info/
+-rw-r--r--   0 lukelele   (501) staff       (20)      613 2024-05-08 18:17:34.000000 pytorch_beacon-0.1.0/PyTorch_Beacon.egg-info/PKG-INFO
+-rw-r--r--   0 lukelele   (501) staff       (20)      295 2024-05-08 18:17:34.000000 pytorch_beacon-0.1.0/PyTorch_Beacon.egg-info/SOURCES.txt
+-rw-r--r--   0 lukelele   (501) staff       (20)        1 2024-05-08 18:17:34.000000 pytorch_beacon-0.1.0/PyTorch_Beacon.egg-info/dependency_links.txt
+-rw-r--r--   0 lukelele   (501) staff       (20)        7 2024-05-08 18:17:34.000000 pytorch_beacon-0.1.0/PyTorch_Beacon.egg-info/top_level.txt
+-rw-r--r--   0 lukelele   (501) staff       (20)      306 2024-05-08 09:48:31.000000 pytorch_beacon-0.1.0/README.md
+drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2024-05-08 18:17:34.952113 pytorch_beacon-0.1.0/beacon/
+-rw-r--r--   0 lukelele   (501) staff       (20)      122 2023-07-21 19:18:08.000000 pytorch_beacon-0.1.0/beacon/__init__.py
+-rw-r--r--   0 lukelele   (501) staff       (20)     7623 2023-10-29 21:20:53.000000 pytorch_beacon-0.1.0/beacon/dataloading.py
+-rw-r--r--   0 lukelele   (501) staff       (20)      933 2023-10-15 15:16:29.000000 pytorch_beacon-0.1.0/beacon/metrics.py
+-rw-r--r--   0 lukelele   (501) staff       (20)     7612 2024-05-08 18:13:05.000000 pytorch_beacon-0.1.0/beacon/module.py
+-rw-r--r--   0 lukelele   (501) staff       (20)     3396 2024-05-05 16:22:36.000000 pytorch_beacon-0.1.0/beacon/training.py
+-rw-r--r--   0 lukelele   (501) staff       (20)     2551 2023-07-19 18:26:46.000000 pytorch_beacon-0.1.0/beacon/utils.py
+-rw-r--r--   0 lukelele   (501) staff       (20)      463 2024-05-08 18:15:20.000000 pytorch_beacon-0.1.0/pyproject.toml
+-rw-r--r--   0 lukelele   (501) staff       (20)       38 2024-05-08 18:17:34.953593 pytorch_beacon-0.1.0/setup.cfg
```

### Comparing `PyTorch-Beacon-0.0.7/LICENCE` & `pytorch_beacon-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `PyTorch-Beacon-0.0.7/beacon/dataloading.py` & `pytorch_beacon-0.1.0/beacon/dataloading.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import os
-import pandas as pd
-import numpy as np
-import torch
-from torchvision import datasets, transforms
-from torch.utils.data import DataLoader, Dataset
-
-
-def from_path(dataset_dir: str, batch_size: int = 32, transform: transforms.Compose = transforms.ToTensor(), shuffle=True, dataset_type=datasets.ImageFolder, pin_memory=True):
-    """
-    Loads a dataset from a given directory path and returns a DataLoader object and the labels of the dataset.
-
-    Args:
-    - dataset_dir (str): The directory path of the dataset.
-    - batch_size (int): The batch size for the DataLoader object. Default is 32.
-    - transform (torchvision.transforms.Compose): The transformation to apply to the dataset. Default is transforms.ToTensor().
-    - shuffle (bool): Whether to shuffle the dataset. Default is True.
-    - dataset_type (torchvision.datasets): The type of dataset to load. Default is datasets.ImageFolder.
-    - pin_memory (bool): Whether to use pinned memory for the DataLoader object. Default is True.
-
-    Returns:
-    - dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded dataset.
-    - labels (list): The labels of the loaded dataset.
-    """
-    dataset = dataset_type(dataset_dir, transform=transform)
-    labels = dataset.classes
-    dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, pin_memory=pin_memory)
-
-    return dataloader, labels
-
-
-def traintest_from_path(trainset_dir: str, testset_dir: str, batch_size: int = 32, transform: transforms.Compose = transforms.ToTensor(), dataset_type=datasets.ImageFolder, pin_memory=True):
-    """
-    Loads train and test datasets from given directory paths and returns DataLoader objects and the labels of the datasets.
-
-    Args:
-    - train_dir (str): The directory path of the train dataset.
-    - test_dir (str): The directory path of the test dataset.
-    - batch_size (int): The batch size for the DataLoader objects. Default is 32.
-    - transform (torchvision.transforms.Compose): The transformation to apply to the datasets. Default is transforms.ToTensor().
-    - shuffle (bool): Whether to shuffle the datasets. Default is True.
-    - dataset_type (torchvision.datasets): The type of dataset to load. Default is datasets.ImageFolder.
-    - pin_memory (bool): Whether to use pinned memory for the DataLoader objects. Default is True.
-
-    Returns:
-    - train_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded train dataset.
-    - test_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded test dataset.
-    - labels (list): The labels of the loaded datasets.
-    """
-    trainset = dataset_type(trainset_dir, transform=transform)
-    testset = dataset_type(testset_dir, transform=transform)
-    labels = trainset.classes
-
-    if trainset.classes == testset.classes:
-        trainloader = DataLoader(trainset, batch_size=batch_size, shuffle=True, pin_memory=pin_memory)
-        testloader = DataLoader(testset, batch_size=batch_size, shuffle=False, pin_memory=pin_memory)
-
-        return trainloader, testloader, labels
-    else:
-        print("Error: trainset and testset classes do not match")
-
-
-class DatasetFromDF(Dataset):
-    """
-    A custom Dataset class that takes a pandas DataFrame as input.
-    
-    Args:
-    - dataframe (pandas.DataFrame): The input DataFrame containing the data.
-    - label_column (str): The name of the column containing the labels. If empty, the first column is used as the label column.
-    
-    Returns:
-    - tuple: A tuple containing the features and labels.
-    """
-    def __init__(self, dataframe, label_column="", transform=None):
-        self.dataframe = pd.DataFrame()
-        self.transform = transform
-
-        if label_column != dataframe.columns[0]:
-            if label_column == "":
-                self.dataframe["index"] = dataframe.index.values
-
-                for col in dataframe.columns:
-                    self.dataframe[col] = dataframe[col]
-            else:
-                self.dataframe[label_column] = dataframe[label_column]
-
-                for col in dataframe.columns:
-                    if col != label_column:
-                        self.dataframe[col] = dataframe[col]
-        else:
-            self.dataframe = dataframe
-
-
-    def __getitem__(self, index):
-        row = self.dataframe.iloc[index].values
-
-        if self.transform:
-            features = self.transform(torch.tensor(row[1:], dtype=torch.float32))
-        else:
-            features = torch.tensor(row[1:], dtype=torch.float32)
-        label = torch.tensor(row[0], dtype=torch.long)
-        return features, label
-
-
-    def __len__(self):
-        return len(self.dataframe)
-
-
-def from_df(dataframe, label_column="", batch_size: int = 32, transform: transforms.Compose = None, shuffle=True, pin_memory=True):
-    """
-    Loads a dataset from a given pandas DataFrame and returns a DataLoader object and the labels of the dataset.
-    The dataframe must contain one column for the labels and the rest of the columns for the features.
-
-    Args:
-    - dataframe (pandas.DataFrame): The pandas DataFrame containing the dataset.
-    - label_column (str): The name of the column containing the labels of the dataset. Default is an empty string.
-    - batch_size (int): The batch size for the DataLoader object. Default is 32.
-    - transform (torchvision.transforms.Compose): The transformation to apply to the dataset. Default is transforms.ToTensor().
-    - shuffle (bool): Whether to shuffle the dataset. Default is True.
-    - pin_memory (bool): Whether to use pinned memory for the DataLoader object. Default is True.
-
-    Returns:
-    - dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded dataset.
-    - labels (list): The labels of the loaded dataset.
-    """
-    dataset = DatasetFromDF(dataframe, label_column=label_column, transform=transform)
-    dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, pin_memory=pin_memory)
-
-    return dataloader
-
-
-def traintest_from_df(train_dataframe, test_dataframe, label_column="", batch_size: int = 32, transform: transforms.Compose = None, pin_memory=True):
-    """
-    Loads train and test datasets from given pandas DataFrames and returns DataLoader objects and the labels of the datasets.
-
-    Args:
-    - train_dataframe (pandas.DataFrame): The pandas DataFrame containing the train dataset.
-    - test_dataframe (pandas.DataFrame): The pandas DataFrame containing the test dataset.
-    - label_column (str): The name of the column containing the labels of the dataset. Default is an empty string.
-    - batch_size (int): The batch size for the DataLoader objects. Default is 32.
-    - transform (torchvision.transforms.Compose): The transformation to apply to the datasets. Default is transforms.ToTensor().
-    - pin_memory (bool): Whether to use pinned memory for the DataLoader objects. Default is True.
-
-    Returns:
-    - train_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded train dataset.
-    - test_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded test dataset.
-    - labels (list): The labels of the loaded datasets.
-    """
-    trainset = DatasetFromDF(train_dataframe, label_column=label_column, transform=transform)
-    testset = DatasetFromDF(test_dataframe, label_column=label_column, transform=transform)
-
-
-    trainloader = DataLoader(trainset, batch_size=batch_size, shuffle=True, pin_memory=pin_memory)
-    testloader = DataLoader(testset, batch_size=batch_size, shuffle=False, pin_memory=pin_memory)
-    return trainloader, testloader
+import os
+import pandas as pd
+import numpy as np
+import torch
+from torchvision import datasets, transforms
+from torch.utils.data import DataLoader, Dataset
+
+
+def from_path(dataset_dir: str, batch_size: int = 32, transform: transforms.Compose = transforms.ToTensor(), shuffle=True, dataset_type=datasets.ImageFolder, pin_memory=True):
+    """
+    Loads a dataset from a given directory path and returns a DataLoader object and the labels of the dataset.
+
+    Args:
+    - dataset_dir (str): The directory path of the dataset.
+    - batch_size (int): The batch size for the DataLoader object. Default is 32.
+    - transform (torchvision.transforms.Compose): The transformation to apply to the dataset. Default is transforms.ToTensor().
+    - shuffle (bool): Whether to shuffle the dataset. Default is True.
+    - dataset_type (torchvision.datasets): The type of dataset to load. Default is datasets.ImageFolder.
+    - pin_memory (bool): Whether to use pinned memory for the DataLoader object. Default is True.
+
+    Returns:
+    - dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded dataset.
+    - labels (list): The labels of the loaded dataset.
+    """
+    dataset = dataset_type(dataset_dir, transform=transform)
+    labels = dataset.classes
+    dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, pin_memory=pin_memory)
+
+    return dataloader, labels
+
+
+def traintest_from_path(trainset_dir: str, testset_dir: str, batch_size: int = 32, transform: transforms.Compose = transforms.ToTensor(), dataset_type=datasets.ImageFolder, pin_memory=True):
+    """
+    Loads train and test datasets from given directory paths and returns DataLoader objects and the labels of the datasets.
+
+    Args:
+    - train_dir (str): The directory path of the train dataset.
+    - test_dir (str): The directory path of the test dataset.
+    - batch_size (int): The batch size for the DataLoader objects. Default is 32.
+    - transform (torchvision.transforms.Compose): The transformation to apply to the datasets. Default is transforms.ToTensor().
+    - shuffle (bool): Whether to shuffle the datasets. Default is True.
+    - dataset_type (torchvision.datasets): The type of dataset to load. Default is datasets.ImageFolder.
+    - pin_memory (bool): Whether to use pinned memory for the DataLoader objects. Default is True.
+
+    Returns:
+    - train_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded train dataset.
+    - test_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded test dataset.
+    - labels (list): The labels of the loaded datasets.
+    """
+    trainset = dataset_type(trainset_dir, transform=transform)
+    testset = dataset_type(testset_dir, transform=transform)
+    labels = trainset.classes
+
+    if trainset.classes == testset.classes:
+        trainloader = DataLoader(trainset, batch_size=batch_size, shuffle=True, pin_memory=pin_memory)
+        testloader = DataLoader(testset, batch_size=batch_size, shuffle=False, pin_memory=pin_memory)
+
+        return trainloader, testloader, labels
+    else:
+        print("Error: trainset and testset classes do not match")
+
+
+class DatasetFromDF(Dataset):
+    """
+    A custom Dataset class that takes a pandas DataFrame as input.
+    
+    Args:
+    - dataframe (pandas.DataFrame): The input DataFrame containing the data.
+    - label_column (str): The name of the column containing the labels. If empty, the first column is used as the label column.
+    
+    Returns:
+    - tuple: A tuple containing the features and labels.
+    """
+    def __init__(self, dataframe, label_column="", transform=None):
+        self.dataframe = pd.DataFrame()
+        self.transform = transform
+
+        if label_column != dataframe.columns[0]:
+            if label_column == "":
+                self.dataframe["index"] = dataframe.index.values
+
+                for col in dataframe.columns:
+                    self.dataframe[col] = dataframe[col]
+            else:
+                self.dataframe[label_column] = dataframe[label_column]
+
+                for col in dataframe.columns:
+                    if col != label_column:
+                        self.dataframe[col] = dataframe[col]
+        else:
+            self.dataframe = dataframe
+
+
+    def __getitem__(self, index):
+        row = self.dataframe.iloc[index].values
+
+        if self.transform:
+            features = self.transform(torch.tensor(row[1:], dtype=torch.float32))
+        else:
+            features = torch.tensor(row[1:], dtype=torch.float32)
+        label = torch.tensor(row[0], dtype=torch.long)
+        return features, label
+
+
+    def __len__(self):
+        return len(self.dataframe)
+
+
+def from_df(dataframe, label_column="", batch_size: int = 32, transform: transforms.Compose = None, shuffle=True, pin_memory=True):
+    """
+    Loads a dataset from a given pandas DataFrame and returns a DataLoader object and the labels of the dataset.
+    The dataframe must contain one column for the labels and the rest of the columns for the features.
+
+    Args:
+    - dataframe (pandas.DataFrame): The pandas DataFrame containing the dataset.
+    - label_column (str): The name of the column containing the labels of the dataset. Default is an empty string.
+    - batch_size (int): The batch size for the DataLoader object. Default is 32.
+    - transform (torchvision.transforms.Compose): The transformation to apply to the dataset. Default is transforms.ToTensor().
+    - shuffle (bool): Whether to shuffle the dataset. Default is True.
+    - pin_memory (bool): Whether to use pinned memory for the DataLoader object. Default is True.
+
+    Returns:
+    - dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded dataset.
+    - labels (list): The labels of the loaded dataset.
+    """
+    dataset = DatasetFromDF(dataframe, label_column=label_column, transform=transform)
+    dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, pin_memory=pin_memory)
+
+    return dataloader
+
+
+def traintest_from_df(train_dataframe, test_dataframe, label_column="", batch_size: int = 32, transform: transforms.Compose = None, pin_memory=True):
+    """
+    Loads train and test datasets from given pandas DataFrames and returns DataLoader objects and the labels of the datasets.
+
+    Args:
+    - train_dataframe (pandas.DataFrame): The pandas DataFrame containing the train dataset.
+    - test_dataframe (pandas.DataFrame): The pandas DataFrame containing the test dataset.
+    - label_column (str): The name of the column containing the labels of the dataset. Default is an empty string.
+    - batch_size (int): The batch size for the DataLoader objects. Default is 32.
+    - transform (torchvision.transforms.Compose): The transformation to apply to the datasets. Default is transforms.ToTensor().
+    - pin_memory (bool): Whether to use pinned memory for the DataLoader objects. Default is True.
+
+    Returns:
+    - train_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded train dataset.
+    - test_dataloader (torch.utils.data.DataLoader): The DataLoader object for the loaded test dataset.
+    - labels (list): The labels of the loaded datasets.
+    """
+    trainset = DatasetFromDF(train_dataframe, label_column=label_column, transform=transform)
+    testset = DatasetFromDF(test_dataframe, label_column=label_column, transform=transform)
+
+
+    trainloader = DataLoader(trainset, batch_size=batch_size, shuffle=True, pin_memory=pin_memory)
+    testloader = DataLoader(testset, batch_size=batch_size, shuffle=False, pin_memory=pin_memory)
+    return trainloader, testloader
```

### Comparing `PyTorch-Beacon-0.0.7/beacon/metrics.py` & `pytorch_beacon-0.1.0/beacon/metrics.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import torch
-
-
-def categorical_accuracy(y_pred_logit, y_true):
-    """
-    Calculates the categorical accuracy of the predicted logits.
-
-    Args:
-    - y_pred_logit: predicted logits
-    - y_true: true labels
-
-    Returns:
-    - accuracy: categorical accuracy of the predicted logits
-    """
-    y_prob = torch.softmax(y_pred_logit, dim=1)
-    y_pred = torch.argmax(y_prob, dim=1)
-    correct = (y_pred == y_true).float()
-    accuracy = correct.sum() / len(correct)
-
-    return accuracy
-
-
-def binary_accuracy(y_pred_logit, y_true):
-    """
-    Calculates the binary accuracy of the predicted logits.
-
-    Args:
-    - y_pred_logit: predicted logits
-    - y_true: true labels
-
-    Returns:
-    - accuracy: binary accuracy of the predicted logits
-    """
-    y_prob = torch.sigmoid(y_pred_logit)
-    y_pred = torch.round(y_prob)
-    correct = (y_pred == y_true).float()
-    accuracy = correct.sum() / len(correct)
-
-    return accuracy
+import torch
+
+
+def categorical_accuracy(y_pred_logit, y_true):
+    """
+    Calculates the categorical accuracy of the predicted logits.
+
+    Args:
+    - y_pred_logit: predicted logits
+    - y_true: true labels
+
+    Returns:
+    - accuracy: categorical accuracy of the predicted logits
+    """
+    y_prob = torch.softmax(y_pred_logit, dim=1)
+    y_pred = torch.argmax(y_prob, dim=1)
+    correct = (y_pred == y_true).float()
+    accuracy = correct.sum() / len(correct)
+
+    return accuracy
+
+
+def binary_accuracy(y_pred_logit, y_true):
+    """
+    Calculates the binary accuracy of the predicted logits.
+
+    Args:
+    - y_pred_logit: predicted logits
+    - y_true: true labels
+
+    Returns:
+    - accuracy: binary accuracy of the predicted logits
+    """
+    y_prob = torch.sigmoid(y_pred_logit)
+    y_pred = torch.round(y_prob)
+    correct = (y_pred == y_true).float()
+    accuracy = correct.sum() / len(correct)
+
+    return accuracy
```

### Comparing `PyTorch-Beacon-0.0.7/beacon/utils.py` & `pytorch_beacon-0.1.0/beacon/utils.py`

 * *Files identical despite different names*

