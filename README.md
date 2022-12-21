# BAGCN-Covid19

Access to the data and code: https://doi.org/10.5281/zenodo.6361963


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
@article{meng2022bilateral,
  title={Bilateral adaptive graph convolutional network on CT based Covid-19 diagnosis with uncertainty-aware consensus-assisted multiple instance learning},
  author={Meng, Yanda and Bridge, Joshua and Addison, Cliff and Wang, Manhui and Merritt, Cristin and Franks, Stu and Mackey, Maria and Messenger, Steve and Sun, Renrong and Fitzmaurice, Thomas and others},
  journal={Medical Image Analysis},
  pages={102722},
  year={2022},
  publisher={Elsevier}
}

