# HindiNLPTools

A specialized NLP library which provides tools to perform basic NLP tasks on Hindi Datasets. Currently, the library supports 
<ul>
  <li> <b> Named Entity Recognition </b>: The Library provides NER support to tag hindi sentences. Further you can apply NER to sentences in textfiles with running only one line of code. If you wish to train youe own NER model, you can do so without writing any script but in one line of code.</li>
  <li> <b> Part-Of-Speech Tagger </b> : </li>
  <li> <b> AutoClassifier </b> : Train your models on classification datasets just in one line of code. Finetune model using custom parameters</li>
<ul>
  
## NER Tagger
The NER Tagger identifies various parts of sentences and tags them with the type of entity they could represent. Currently the tags supported by our model are
<table> 
  <tr> <th>  Heading </th> <th> Tag Type  </th></tr>
  <tr> <td>  NEP </td> <td> Person  </td></tr>
  <tr> <td>  NED </td> <td> Designation  </td> </tr>
  <tr> <td>  NEO </td> <td> Object  </td> </tr>
  <tr> <td>  NEA </td> <td> Abbreviation  </td> </tr>
  <tr> <td>  NEB </td> <td> Brand  </td> </tr>
  <tr> <td>  NETP </td> <td> Title-Person  </td> </tr>
  <tr> <td>  NETO </td> <td> Title-Object </td> </tr>
  <tr> <td>  NEL </td> <td> Location </td> </tr>
  <tr> <td>  NETI </td> <td> Time </td> </tr>
  <tr> <td>  NEN </td> <td> Number </td> </tr>
  <tr> <td> NEM </td> <td> Measure </td> </tr>
  <tr> <td>  NETE </td> <td> Terms </td> </tr>
</table>

In order to use the Tagger, for one sentence 
```python 
from HindiNLPTools.HindiNer import NER

detect_ner = NER()
sentence = detect_ner.Predict("अविनाश आगरा में रहता है")
print(sentence)
 ```
 Print the sentence to see what the tagger found. Furthermore 
 
