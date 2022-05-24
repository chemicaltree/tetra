# TETRA (Text Revision of ACL papers) corpus
Last updated: May 24th, 2022

TETRA consists of documen-level revisions for the articles published at ACL-related venues, and designed based on an annotation scheme that can handle edit types beyond sentences (such as argument flow) in addition to conventional word- and phrase-level edit types.




See [the paper](https://arxiv.org/abs/2205.11484) for more information.


# Data format
The dataset is formatted in xml, consisting of one xml file per paper. Here's sample of annotations in the dataset:

![example_of_annotation](https://user-images.githubusercontent.com/99496763/169949216-f7a65ec5-3935-40bf-81ba-b3d54e15820d.png)

Each file contains the following information in xml tags.
- meta information
  - `doc id`: ID of the paper (ACL Anthology)
  - `editor`: ID of the revised human expert
  - `format`: venues (conference (Conf) or workshop (WS))
  - `position`: first author's position (Non-student (NS) or Student (S))
  - `region`: region of the affiliation (Native (N) or Non-native (NN))
- edit information
  - `edit type`: edit type
  - `crr`: edit instance by human expert
  - `comments`: rationale comments

# Citation
Thank you for your interest in our dataset. If you use it in your research, please cite:]

```
@misc{mita2022automated,
      title={Towards Automated Document Revision: Grammatical Error Correction, Fluency Edits, and Beyond}, 
      author={Masato Mita and Keisuke Sakaguchi and Masato Hagiwara and Tomoya Mizumoto and Jun Suzuki and Kentaro Inui},
      year={2022},
      eprint={2205.11484},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
