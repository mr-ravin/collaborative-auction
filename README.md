# collaborative-auction
This repository contains the source codes of our research paper in economics titled: "Addictive auctions: using lucky-draw and gambling addiction to increase participation during auctioning".

#### Paper Title: Addictive auctions: Using lucky-draw and gambling addiction toincrease participation during auctioning

#### Author: [Ravin Kumar](https://mr-ravin.github.io)

#### Publication: 18th January 2021.

#### Publication Journal: [International Journal of Management Research and Economics](https://www.svedbergopen.com/journals/International-Journal-of-Management-Research-and-Economics/About-the-Journal/)

#### Publication House: [SvedbergOpen](https://www.svedbergopen.com)

#### Publication link: https://www.svedbergopen.com/files/1612268008_(5)_IJMRE28112020MTN007_(p_68-74).pdf

#### Publication copy: https://mr-ravin.github.io/economist/static/media/AddictiveAuctions.fea57be7.pdf

#### Cite as:

```
Ravin Kumar (2021). Addictive auctions: Using lucky-draw and gambling addiction to increase participation during auctioning.
International Journal of Management Research and Economics. 1(1),68-74.
```

#### Doi: https://doi.org/10.51483/IJMRE.1.1.2021.68-74

#### Also available on Elsevier-SSRN eJournals: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3795556

- Behavioral & Experimental Economics eJournal.
- Microeconomics: Welfare Economics & Collective Decision-Making eJournal.
- Microeconomics: Production, Market Structure & Pricing eJournal.

####  Earlier Preprints:

- OSF Preprints : https://doi.org/10.31219/osf.io/darvs
- Cornell University LIbrary, arXiv.org : https://arxiv.org/abs/1906.03237

 ### Steps for using the library
```python
import coauction
# total_candidates : total number of participants
# bidding_sequence: arrary containing timeseries data in format [[candidate_id,candidate_offer],[candidate_id,candidate_offer] ....]
# relation_list: array containing relationship in form of [[sender,receiver],..] here 1 represents the person who won the bidding, 2 repreents the second last bidding candidate etc.
# alpha: it determine the discount ratio for each relationship present in relation_list
results=coauction.response(total_candidates,bidding_sequence,relation_list,alpha)
# results[0] contains complete list of amount each candidate gets, and results[1] contains the amount in form of a dictionary,
# with candidate_id as key, and amount as value.
```

### Installing module using PyPi:
```python
pip install coauction
```
In our system, the candidate_id begins with 1 in the dictionary based response.

```python
Copyright (c) 2019 Ravin Kumar
Website: https://mr-ravin.github.io

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, 
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the 
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the 
Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```
