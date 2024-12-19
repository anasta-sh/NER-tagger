# NER-tagger

This is a unversity project implementing a NER Tagger with PyTorch. It uses the English CONLL 2003 dataset.

**Dataset description**
It encodes each token on a single line followed by its annotation:
(token,tag,chunk,named entity)
The NER tags follow the IOB convention:
* **I**: **Inside** (part of a named entity);
* **B**: **Begin** (starting a new entity);
* **O**: **Outside** (not part of a named entity).
  
The **I** and **B** tags are followed by a specifier that identifies the type of the entity, such as:
* **PER**: Person
* **ORG**: Organization
*	**LOC**: Location

The project has a basic NER tag model and an improved version with **attention layer**, **part-of-speech tag embeddings as additional inputs**, **convolutional neural network (CNN) over character embeddings** (for better recognition of OOV words). After improvements the valid accuracy increased by 2.76% from 93.58% to 96.34%, demonstrating that the improved version is more efficient and accurate in recognizing named entities.



