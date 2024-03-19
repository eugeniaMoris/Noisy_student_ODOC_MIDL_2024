# Semi-supervised learning with Noisy Students improves domain generalization in optic disc and cup segmentation in uncropped fundus images
by Eugenia Moris, Ignacio Larrabide and Jos{\'e} Ignacion Orlando

## Abstract

<p align="justify">
Automated optic disc (OD) and cup (OC) segmentation in fundus images has been widely explored for computer-aided diagnosis of glaucoma. 
However, existing models usually suffer from drops in performance when applied on images significantly different than those used for training.
Several domain generalization strategies have been introduced to mitigate this issue, although they are trained and evaluated using images manually cropped around the optic nerve head. 
This operation eliminates most sources of domain variation, therefore overestimating their actual ability to cope with new, unseen patterns. 
In this paper, we analyze the most recent and accurate methods for domain generalization in OD/OC segmentation by applying them on uncropped fundus pictures, observing notorious degradations in their performance when trained and evaluated under this setting.
To overcome their drawbacks, we also introduce a simple semi-supervised learning approach for domain generalization based on the Noisy Student framework.
Using a Teacher model trained on a combination of domains, we pseudo-labeled a dataset of 18.000 originally unlabeled images that are then used for training a Student model.
This semi-supervised setting allowed the Student network to capture additional sources of variability while retaining the original cues and patterns used by the Teacher through the weak annotations.
Our results on eight different public datasets show improvements in every unseen domain over all alternative methods.
</p>


![Alt text](https://github.com/eugeniaMoris/Noisy_student_ODOC_MIDL_2024/blob/main/method.png "Metodology used")

## Objetive
<p align="justify">
We created this repository to produce a series of segmentations for various public datasets. Our goal is to provide a platform for anyone to compare their models with ours. The repository includes the segmentations created by our Teacher as well as two Students who were trained with the purpose of improving domain generalization in optic disc and cup segmentation. 
</p>

The public datasets used in the test are listed in the table below.



| Dataset    | Number of samples | 
|:----------:|:-----------------:|
| BOSCH      | 41    |
| FORUS      | 31    |
| REMIDIO    | 264   |
| DRISHTI    | 50    |
| REFUGE     | 400   |
| RIM ONE v3 | 159   |
| ORIGA      | 647   |
| PALM       | 400   |
| AIROGS     | 18000 |




## Citation

```
@inproceedings{moris2024semi,
  title={Semi-supervised learning with Noisy\~{} Students improves domain generalization in optic disc and cup segmentation in uncropped fundus images},
  author={Moris, Eugenia and Larrabide, Ignacio and Orlando, Jos{\'e} Ignacio},
  booktitle={Medical Imaging with Deep Learning},
  year={2024}
}
```

## Contact

email: emoris@pladema.exa.unicen.edu.ar

web: [Yatiris Group](https://yatiris.github.io/people/eugenia_moris/index.html)


