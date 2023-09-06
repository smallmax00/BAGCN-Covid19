# BAGCN-Covid19

Access to the data and code: https://doi.org/10.5281/zenodo.6361963

The pre-segmented cell, MosMed and CovidCT data can be found here: [data](https://drive.google.com/drive/folders/1xiYo53qsmv9Db-RD_XMgzvZwyFpes3Zw?usp=sharing)


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

@article{zhang2020clinically,
  title={Clinically applicable AI system for accurate diagnosis, quantitative measurements, and prognosis of {COVID}-19 pneumonia using computed tomography},
  author={Zhang, Kang and Liu, Xiaohong and Shen, Jun and Li, Zhihuan and Sang, Ye and Wu, Xingwang and Zha, Yunfei and Liang, Wenhua and Wang, Chengdi and Wang, Ke and others},
  journal={Cell},
  volume={181},
  number={6},
  pages={1423--1433},
  year={2020},
  publisher={Elsevier}
}

@article{morozov2020mosmeddata,
  title={Mosmeddata: data set of 1110 chest {CT} scans performed during the {COVID}-19 epidemic},
  author={Morozov, Sergey P and Andreychenko, Anna E and Blokhin, Ivan A and Gelezhe, Pavel B and Gonchar, Anna P and Nikolaev, Alexander E and Pavlov, Nikolay A and Chernina, Valeria Yu and Gombolevskiy, Victor A},
  journal={Digital Diagnostics},
  volume={1},
  number={1},
  pages={49--59},
  year={2020}
}

@article{RAHIMZADEH2021102588,
title = {A fully automated deep learning-based network for detecting {COVID}-19 from a new and large lung {CT} scan dataset},
journal = {Biomedical Signal Processing and Control},
pages = {102588},
year = {2021},
issn = {1746-8094},
doi = {https://doi.org/10.1016/j.bspc.2021.102588},
url = {https://www.sciencedirect.com/science/article/pii/S1746809421001853},
author = {Rahimzadeh, Mohammad and Attar, Abolfazl and Sakhaei, Seyed Mohammad},
}

