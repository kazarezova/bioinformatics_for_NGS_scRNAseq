ноутбук Google Colaboratory: https://colab.research.google.com/drive/1AbJqasrnccEt90igUeBog28gQeEzFAHa?usp=sharing

использованные данные: https://drive.google.com/file/d/1lrb2Pxc-oN9GKc3yXrU4OKlLCnI7utUZ/view?usp=sharing

взяты из статьи Bakken, T.E., Jorstad, N.L., Hu, Q. et al. Comparative cellular analysis of motor cortex in human, marmoset and mouse. Nature 598, 111–119 (2021). https://doi.org/10.1038/s41586-021-03465-8

с сайта CELLxGENE: https://cellxgene.cziscience.com/e/9b686bb6-1427-4e13-b451-7ee961115cf9.cxg/

что исправлено:
- оставила один батч (одного человека)
- убрала второй логариф
- отрисовала cell_type из статьи
- сделала подсчет ARI и NMI с перебором resolution в leiden, везде теперь использованы эти метрики
- adata_2 = adata_1 заменила на adata_2 = adata_1.copy()
- для варианта пайплайна без PCA убрала PCA из sc.pp.neighbors
- доделала вариант с SVD
