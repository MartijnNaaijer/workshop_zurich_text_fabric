# Example Queries in the BHSA

### BHSA feature documentation:
https://etcbc.github.io/bhsa

### Lexicon:
https://shebanq.etcbc.vu.nl OR https://shebanq.ancient-data.org

### Search documentation:
https://annotation.github.io/text-fabric/tf/about/searchusage.html

### Tutorials:
https://github.com/ETCBC/bhsa/blob/master/tutorial/search.ipynb
https://github.com/ETCBC/bhsa/blob/master/tutorial/searchAdvanced.ipynb




Example queries:

word


word lex=MCH/


word lex=MCH=/


clause
  word lex=MCH=/


clause 
  word lex=HLK[


clause 
  word lex=JHWH/|>LHJM/


clause 
  word lex=HLK[ ps=p1 vs=piel vt=perf


clause
  word lex=HLK[ vs* # vs now in exported dataset


clause
  word g_cons=HLKTJ  # Note ketiv qere in 2Kings 4:23 and Jeremiah 31:21


clause
  word g_cons~^B..$


clause
  word sp=verb


clause
  word sp#verb


clause
  word uvf=H


clause
  word language=Hebrew 


clause
  phrase typ=NP


clause
  phrase function=Subj


clause
  phrase function=Subj
  phrase function=Objc


clause
  phrase function=Subj
    word lex=MCH=/


clause
  phrase function=Subj
    word lex=MCH=/
    word lex=>HRN/


clause
    word lex=MCH=/
    > word lex=>HRN/


clause
    word lex=MCH=/
    < word lex=>HRN/


clause
  phrase function=Subj
  > phrase function=Objc


clause
  word lex=JHWH/
  :> word lex=>MR[


clause
  word lex=JHWH/
  <: word lex=>MR[


clause
  =: word lex=HLK[


clause
  := word lex=HLK[


clause
  :: word lex=HLK[


clause
  word lex=MCH=/
  :2> word sp=verb # try also :3> word sp=verb


book book=Exodus
  chapter chapter=3
    verse verse=11
      clause kind=NC


book book=Deuteronomium
  clause kind=NC


book book@en=Deuteronomy
  clause kind=NC


book book@da=1.Kongebog
  clause kind=NC


clause
  clause_atom
  < clause_atom


clause
/where/
  phrase
/have/
  /without/
     function=Objc
  /-/
/-/

clause
/where/
  phrase
/have/
     function#Objc
/-/
