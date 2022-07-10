# Summary

The Basque UD treebank is based on a automatic conversion from part of the Basque Dependency Treebank (BDT), created at the University of of the Basque Country by the IXA NLP research group. The treebank consists of 8.993 sentences (121.443 tokens) and covers mainly literary and journalistic texts.

# Introduction

The Basque UD treebank is based on a automatic conversion from part of the Basque Dependency Treebank (BDT) (Aduriz et al., 2003), created at the University of of the Basque Country by the IXA NLP research group. The treebank consists of 5274 sentences (60563 tokens) and covers mainly literary and journalistic texts. The Basque language can be described as a morphologically rich, agglutinative language with a high capacity of generating inflected word-forms, with free constituent order of sentence elements. It can be considered a head-final language, as the syntactic head of phrases is located at the end of the last word of the phrase, in the form of a suffix. BDT is a pure dependency treebank from its original design, annotated in the CoNLL-X format, and it shares with UD a lexicalist hypothesis in syntax, where dependencies occur between whole individual wordforms. Under this lexicalist approach, each word shows several morphosyntactic associated features, corresponding to affixes (prefixes and suffixes) attached to the base forms, such as case (there are 14 morphological cases in Basque), number, definiteness or type of subordinate sentence (adversative, conditional, ...). These suffixes usually appear as separated wordforms in non agglutinative languages. The last version of BDT contains 150,000 tokens forming 11,225 sentences, with 1.3% of non-projective arcs. BDT encodes 16 different POS and 28 dependencies. Although BDT was in accord with many UD guidelines, the process was not trivial, converting around 80% of the tokens (121.443 tokens). The set of remaining sentences correspond to either special cases not accounted by the conversion rules or other types of less frequent phenomena which have not been dealt with at the moment.


# Acknowledgments

The conversion of the original treebank has been performed by Aitziber Atutxa, Iakes Goenaga and Koldo Gojenola at University of the Basque Country (EHU/UPV). In contrast, the conversion of the UD treebank v1.2 to v2.0 has been performed by Dan Zeman. We thank everyone who has collaborate in the transformation of the Basque Dependency Treebank.

Sentences were randomized and divided in 60-20-20 splits for the train, dev and test files, repectively.

# References

Aranzabe M., Atutxa A., Bengoetxea K., Díaz de Ilarraza A., Goenaga I., Gojenola K., Uria L. 2015 Automatic Conversion of the Basque Dependency Treebank to Universal Dependencies. 14th International Workshop on Treebanks and Linguistic Theories, TLT 2015, Warsaw , Poland, December 11-12.

# Changelog

* 2022-11-15 v2.11
  * Fixed: Only punctuation should be attached via the punct relation; and punctuation should always use it.
  * Fixed: Spurious copulas with wrong UPOS.
  * Fixed: Apposition should go left-to-right.
  * Fixed: Proper nouns are not case markers.
  * Fixed: Dependents of fixed functional expressions, if any, should be attached to the first node.
  * Fixed: Pseudo-copulas such as ibili, geratu, sartu, sortu, onartu, ari_izan.
  * Fixed: A predicate can have two subjects only if one of them is :outer and the predicate heads a clause which is a predicate of the outer clause.
  * Fixed: NOUN, ADJ, DET, INTJ should not be attached as mark.
  * Fixed: NOUN, PROPN, PRON, NUM, VERB, INTJ, X cannot be attached as advmod.
  * Fixed: Punctuation should be leaf and should not cause non-projectivity.
  * Fixed: Nodes attached as cc should be leaves.
  * Fixed: NOUN, PROPN, ADJ, NUM, VERB, ADV, PART cannot be attached as det.
  * Fixed: Ordinal numerals should be ADJ, not NUM.
  * Fixed: Nodes attached as case or mark should be leaves.
  * Fixed: Nodes attached as aux should be AUX, not VERB.
  * Fixed: Nodes attached as cop should be leaves.
  * Fixed: A clause has at most one subject.
  * Fixed: A verb (VERB, AUX) always has a VerbForm.
* 2018-04-15 v2.2
  * Repository renamed from UD_Basque to UD_Basque-BDT.
* 2016-12-01 v2.0
  * We adapt the v1.2 treebank to v2.0 treebank guidelines
* 2015-11-15 v1.2
  * The size increased since v1.1 after adding a new set of sentences from BDT which include previously non-treated phenomena like multiwords, entities and complex post-positions
  * Some errors in POS have been fixed (related to some SCONJ that were in fact Verbs)
* 2015-05-15 v1.1
  * First release in UD


=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v1.1
License: CC BY-NC-SA 3.0
Includes text: yes
Genre: news
Lemmas: automatic
UPOS: converted from manual
XPOS: converted from manual
Features: converted from manual
Relations: converted from manual
Contributors: Aranzabe, Maria Jesus; Atutxa, Aitziber; Bengoetxea, Kepa; Diaz de Ilarraza, Arantza; Goenaga, Iakes; Gojenola, Koldo; Uria, Larraitz
Contributing: elsewhere
Contact: koldo.gojenola@ehu.eus
===============================================================================

