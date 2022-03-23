# BAGCN-Covid19


**Dataset**:  

--We provide the annotated 7768 masks of C-19 CT slices, also we have provided the indices of the training&val, test datasets for two evaluations of learning ability (Cell) and generalization ability (cell+mosmed+covid-ct). The masks are in the file of masks.zip and the data indices are in the file of code_data_pre-trained-models.zip. 

**Implementation code**:  

```
Prepare your data, and split them as the index stated in ./data_index
```

**UC-MIL**

**train**

```
run UC-MIL-train.py
```

**BA-GCN**

**train**
```
prepare data for BA-GCN using the pre-trained UC-MIL model, select the top 16 slicesf ro each CT scan.
```

```
run BA-GCN-train.py
```



