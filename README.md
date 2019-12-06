# collaborative-auction
This repository contains the source codes of our research paper in economics titled: "Addictive Auctions: using lucky-draw and gambling addiction to increase participation during auctioning".

#### Author: [Ravin Kumar](https://mr-ravin.github.io)

#### Elsevier-SSRN eJournals:

Research Paper link : https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3488563

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
In our system candidate_id begins with 1, in dictionary based response.

#### Note: This work can be used freely for academic research work and individual non-commercial projects, please do provide citation and/or deserved credits to this work. For Industrial and commercial use permission is required from the Author.
