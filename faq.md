# Questions

### _How are NER systems usually built?_
  - Though rule-based systems exist, typically NER is framed as a supervised learning problem.  Take a look at sequence tagging models (HMM, CRF, RNN, LSTM, etc.).
  - For feature-based models, here are few commonly used features:
    - word shape for encoding capitalization (ex. Bob -> Xxx, Virginia -> Xxx)
    - PoS tag
    - prefix and suffix
    - the same features for surrounding words
