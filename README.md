The code is to automatically download figures that contain either pathway or network in the figure caption from a list of papers with PMIDs. Pathway figures are stored in output (for paper that has PMCID) and output_noPMCIDs (for paper that only have PMIDs) folders

Nhung Pham 18-06-2021

# Input:
- List of pm ids as data. In this case, the collection from the DM project was used

#Output:
- Pathway figures stored in sub-folder named after the pmid of the original paper
- text file that indicates which pm ids do not contain pathway figures (no_pathway.txt)
- text file that indicates which pm ids cannot be mapped to PMCID (no_found_ids.txt)

#### How to run:

- The main code is in the jupyter notebook file “Download_figures_from_PMC_papers”
- Add input to the function “take_imgs_from_multiple_sites” . Figures will be saved in the output folder in the current directory.
- For pmid that does not have a corresponding pmcid, use the function 'get_from multi_pmids'. Note that the html structure is different for each website, it is more difficult to make a general download for these papers. In this case, manually download is required
