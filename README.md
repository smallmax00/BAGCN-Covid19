# BAGCN-Covid19


**Dataset**:  

--We provide the annotated 7768 masks of C-19 CT slices, also we have provided the indices of the training&val, test datasets for two evaluations of learning ability (Cell) and generalization ability (cell+mosmed+covid-ct). The masks are in the file of masks.zip and the data indices are in the file of code_data_pre-trained-models.zip. 

**Implementation code**:  

```
Prepare your data, and split them as the index stated in ./data_index
```

**UC-MIL**

**train:**

```
run UC-MIL-train.py
```

**BA-GCN**

**train:**
```
prepare data for BA-GCN using the pre-trained UC-MIL model, select the top 16 slicesf ro each CT scan.
```

```
run BA-GCN-train.py
```


**Pre-trained model**.

```
We shared the pre-trained models of UC-MIL and BA-GCN in the folder ./pre-trained_model, for two evaluation settings called './Cell' and 'cell_mosmed_covid_ct'
```

# Citation
If you find our work useful or use our dataset, please cite:
```
@dataset{yanda_meng_2022_6361963,
  author       = {Yanda Meng and
                  Joshua Bridge and
                  Siyu Ren and
                  Cliff Addison and
                  Manhui Wang and
                  Cristin Merritt and
                  Stu Franks and
                  Maria Mackey and
                  Steve Messenger and
                  Renrong Sun and
                  Yitian Zhao and
                  Yalin Zheng},
  title        = {{Dataset \& Code related to article  'Bilateral 
                   Adaptive Graph Convolutional Network on CT based
                   COVID-19 Diagnosis with Uncertainty-Aware
                   Consensus-Assisted Multiple Instance Learning'}},
  month        = mar,
  year         = 2022,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.6361963},
  url          = {https://doi.org/10.5281/zenodo.6361963}
}
