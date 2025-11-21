## [Multimodal Corn Disease Dataset(MCDD)]([WCG-VMamba: A multi-modal classification model for corn disease - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S0168169924012262?via%3Dihub))

### 😕What is it？

**The Multimodal Maize Disease Dataset (MCDD)** is a multi-modal dataset for maize disease classification, and we constructed the MCDD through field shooting and web data search. MCDD contains a total of **4633** corn images, involving **4 categories**:  <u>corn blight, corn rust, corn gray spot, and health images</u>. 

Each corn image contains a corresponding text description, as described in **MCDD/csv/** */ for details. We use the **LLAVA-1. 5-7b** model to use the prompt word "**describe the picture**" for each image to obtain the text description.

### 📁File Structure

The dataset structure is as follows：

```
MCDD
	--csv
		--test
			--test_data.csv
		--train
			--train_data.csv
	--data
		--test
			--Blight
				--Corn_Blight (1).jpg
				--……
			--Common_Rust
				--Corn_Common_Rust (3).jpg
				--……
			--Gray_Leaf_Spot
				--Corn_Gray_Spot (8).jpg
				--……
			--Healthy
				--Corn_Health (11).jpg
				--……
		--train(same structure as test folder)
```

For a csv file under MCDD/csv, each row is a text pair with the following table structure:

```
describe | label | image
```

**describe**: text description of the image

**label**:  image category

**image**: image path

### 🏁Cite Our Work

If our work is useful for your research, please consider citing and give us a star ⭐

```
@article{WANG2025109835,
title = {WCG-VMamba: A multi-modal classification model for corn disease},
journal = {Computers and Electronics in Agriculture},
volume = {230},
pages = {109835},
year = {2025},
issn = {0168-1699},
doi = {https://doi.org/10.1016/j.compag.2024.109835},
url = {https://www.sciencedirect.com/science/article/pii/S0168169924012262},
author = {Haoyang Wang and Mingfang He and Minge Zhu and Genhua Liu},
keywords = {Corn disease, Image-text pairs, Classification, Multimodal, VMamba},
```



