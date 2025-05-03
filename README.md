# US Media Coverage of China: A Comparative Study with Keyword-Assisted Topic Model

Wendy Shi

## Introduction

U.S. media coverage of China has consistently carried a somewhat negative connotation, often framed through the lens of geopolitical rivalry and ideological tension. **Yang and Liu (2012)** found that between 1992 and 2006, U.S. print media frequently portrayed China as a threat, whether military, economic, political, or ideological, based on a qualitative content analysis of major newspapers. Building on their work, this study seeks to explore how U.S. media currently portrays China and to identify key topics emphasized in recent publications and see if these topic goes beyond military, economic, ideology, and politics.

To ensure objectivity, I will compare the coverage of China with that of Japan. Japan is one of the world’s largest economies, a major trading partner in the Asia-Pacific region, and a close U.S. ally, frequently depicted in a more favorable light. By comparing media portrayals of China and Japan, I aim to reveal both distinct differences and shared thematic patterns.
The primary objective of this research is to identify and frame the dominant topics in U.S. media coverage of China. As noted by **Chang et al. (2009)**, traditional topic models such as LDA and STM often yield vague or ambiguous themes, sometimes described as “reading tea leaves”, because they cluster similar words without assigning clear semantic meaning. 

To address this limitation, I adopt a semi-supervised approach using the Keyword-Assisted Topic Model (KeyATM), first proposed by **Eshima and Sasaki (2024)**. This method allows for the manual assignment of topic labels based on a set of predefined keywords, improving interpretability while maintaining flexibility in the modeling process. Our research finds that U.S. media tend to portray China through a more socio-political lens, with coverage focusing on topics such as elections, domestic policies, foreign relations, Asia-Pacific geopolitical tensions, technology, and trade. In contrast, media coverage of Japan leans more toward a geo-cultural perspective. While it also includes some of the socio-political themes mentioned above, there is a noticeably stronger emphasis on entertainment in the coverage of Japan.

## Folder Guide
### `01_Code/`
- `0_NYT_Data_Collection.ipynb` : Python notebook to query New York Time API
- `1_FP_China_STM.qmd`: R file to generate word cloud, NYT lable distributions, `searchk()` for `STM`, and final `STM` results
- `2_FP_China_KeyATM.qmd`: R file to generate keyword distributions, `KeyATM` results, and covariates analysis for China
- `3_FP_Japan_STM.qmd`: `STM` analysis for Japan
- `4_FP_Japan_STM.qmd`: `KeyATM` analysis for Japan

### `02_Code_html/`
All mentioned files in `01_code/`, compiled to html

### `03_Data`
- `China_merged_2024.xlsx`: All data news article analyzed for China
- `Japan_merged_2024.xlsx`: All data news article analyzed for Japan

### `04_Visualiztaions`
This folder contains the visualizations included in the final paper. Please refer to the file names of each image for reference.

### `05_Final_Paper`
This contains the pdf format of the final paper

### `06_Presentation.pdf`
Presentation used for the class

### `07_Original_Proporal`
Note that the methodology has shifted from word embedding to keyword-assisted topic modeling.

  
## Reference
Chang, Jonathan, Jordan Boyd-Graber, Sean Gerrish, Chong Wang, and David M. Blei. 2009. “Reading Tea Leaves: How Humans Interpret Topic Models.” In Proceedings of the 22nd International Conference on Neural Information Pro- cessing Systems (NIPS ’09). 288–96.

Eshima, S., Imai, K., & Sasaki, T. (2024). Keyword‐assisted topic models. American Journal of Political Science, 68(2), 730-750.

Yang, Y. E., & Liu, X. (2012). The ‘China threat’through the lens of US print media: 1992–2006. Journal of Contemporary China, 21(76), 695-711.
