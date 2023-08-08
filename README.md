<!-- ------------------ HEADER ------------------ -->
<!-- Developed and maintained by Genomics Division
<!-- of the Institute of Technology an Renewable Energy (ITER)
<!-- Tenerife, Canary Islands, SPAIN
<!-- See the "Contact us" section to collaborate with us to growth
<!-- this repository. ;=)

<!-- ------------------ SECTION ------------------ -->
<p align="left">
  <a href="https://github.com/genomicsITER/influenza" title="Instituto Tecnológico y de Energ&iacute;as Renovables (ITER) / Institute of Technology and Renewable Energy (ITER)">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/logos_GH.png" width="auto" /> 
      </a>
</p>

# Influenza
A public repository of **Influenza** (Inf) related resources maintained by ITER.

This is the result of a continuous collaborative effort of the following Institutions and Laboratories:
<ul>
 <li><a href="https://www3.gobiernodecanarias.org/sanidad/scs/organica.jsp?idCarpeta=10b3ea46-541b-11de-9665-998e1388f7ed">Servicio de Microbiología, Hospital Universitario Ntra. Sra. de Candelaria</a>, 38010 Santa Cruz de Tenerife, Spain.</li>
 <li><a href="https://fciisc.org/">Fundación Canaria Instituto de Investigación Sanitaria de Canarias</a> at the Research Unit, Hospital Universitario Ntra. Sra. de Candelaria</a>, 38010 Santa Cruz de Tenerife, Spain.</li>
 <li><a href="https://portalciencia.ull.es/grupos/6361/detalle">Laboratorio de Inmunología Celular y Viral</a>, Unidad de Farmacología, Facultad de Medicina, Universidad de La Laguna, 38200 San Cristóbal de La Laguna, Spain.</li>
 <li><a href="https://www.iter.es/areas/area-genomica/">Genomics Division, Instituto Tecnológico y de Energías Renovables</a>, 38600 Santa Cruz de Tenerife, Spain.</li>
</ul>

<hr>
<!-- ------------------ SECTION ------------------ -->

# Table of contents #
<ul>
  <li><a href="#Virological posts">Virological post: A draft of the first genome sequence of MPXV virus associated with the multi-country outbreak in May 2022 from the Canary Islands, Spain</a></li>
  <li><a href="#Bioinformatic pipelines">Bioinformatic pipelines</a></li>
    <ul>
      <li><a href="#Code-Illumina">Code for Illumina short-reads processing</a></li>
      <li><a href="#Code-ONT">Code for Nanopore long-reads processing and hybrid <i>de novo</i> assemby</a></li>
      <li><a href="#List-of-software">List of bioinformatic software used in our pipelines</a></li>
      <li><a href="#Useful-Files">Useful files for the pipelines</a></li>
  </ul>
  <li><a href="#Sequences">Sequences</a></li>
  <li><a href="#How-to-GenBank">How to download sequences and metadata from GenBank</a></li> 
  <li><a href="#DNA-depletion">Enrichment of viral DNA by means of Human & Bacterial DNA depletion</a></li>  
  <li><a href="#Other-repos">Other useful repositories with resources to study MPXV</a></li>
  <li><a href="#References">References</a></li>
  <li><a href="#Acknowledgements">Acknowledgements</a></li>
  <li><a href="#License and Attribution">License and Attribution</a></li>
  <li><a href="#Participating">Participating</a></li>
  <li><a href="#How-to-cite">How to cite this work</a></li>
  <li><a href="#Update logs">Update logs</a></li>
</ul>

<hr>
<!-- ------------------ SECTION 1 ------------------ -->

<a name="Virological posts"></a>
## Virological posts ##

A technical post with the draft of the first genome sequence of MPXV virus associated with the multi-country outbreak in May 2022 from the Canary Islands, Spain has been shared in Virological. Keep reading! [Here.](https://virological.org/t/a-draft-of-the-first-genome-sequence-of-monkeypox-virus-associated-with-the-multi-country-outbreak-in-may-2022-from-the-canary-islands-spain/864)

The first genome sequence of MPXV virus described by us in Virological is phylogenetically related to the multiple viral genomes deposited in NCBI GenBank that correspond to the actual 2022 worldwide outbreak, as shown in Figure 1.

<p align="center">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/figures/Nextstrain-monkeypox_HUNSC_ITER_Figure1.png" width="auto" />
  </a>
</p>

**Figure 1**. A phylogenetic tree depicting the draft MPXV sequence isolated on May 31, 2022 from a patient from the Canary Islands along with NCBI GenBank publicly available sequences computed by a Nextstrain-monkeypox local instance.

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>

<hr>
<!-- ------------------ SECTION 2 ------------------ -->

<a name="Bioinformatic pipelines"></a>
## Bioinformatic pipelines ##

The following diagram (Figure 2) represents a full pipeline used to derive the consensus FASTA sequence of MPXV virus using and combining short- and long-reads technologies (Illumina and Nanopore, respectively).

In the upper part of the diagram, there is a typical pipeline to process short-reads, from the basecalling to the final consensus FASTA sequence, and downstream analysis such as the phylogenetic inference.

In the lower part of the diagram, it is shown a typical pipeline to process long-reads. In addition, it shows how to perform a hybrid *de novo* assembly combining short- and long-reads.

Two consensus MPXV sequences have been obtained and deposited in NCBI GenBank following the described pipeline:
<ul>
  <li>A FASTA sequence derived from the pipeline based on mapping of Illumina short-reads against a MPXV reference genome.</li>
  <li>A FASTA sequence resulting from the consensus of the hybrid *de novo* assembly and a MPXV reference genome to complete uncovered regions.</li>
</ul>

<p align="center">
  <a href="https://www.iter.es" title="Instituto Tecnológico y de Energ&iacute;as Renovables (ITER) / Institute of Technology and Renewable Energy (ITER)">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/INF_pipeline_v1.png" width="auto" /> 
  </a>
</p>

**Figure 2**. Full bioinformatic pipeline to obtain the MPXV sequences and to infer phylogenetic relationships with other MPXV viral genomes available obtained from public repositories.

<hr>

<a name="Code-Illumina"></a>
**Code for Illumina short-reads processing**

<a href="https://github.com/genomicsITER/influenza/blob/main/codes/code_Illumina_pipeline.md"><img src="https://github.com/genomicsITER/influenza/blob/main/images/Code-Window-icon.png" width="32px" /></a>  See a detailed pipeline with examples of command usage for [Illumina short-reads](https://github.com/genomicsITER/influenza/blob/main/codes/code_Illumina_pipeline.md).

<hr>

<a name="Code-ONT"></a>
**Code for Nanopore long-reads processing and hybrid *de novo* assemby**

<a href="https://github.com/genomicsITER/monkeypox/blob/main/codes/code_ONT-and-HybridAssembly_pipeline.md"><img src="https://github.com/genomicsITER/monkeypox/blob/main/images/Code-Window-icon.png" width="32px" /></a>  See a detailed pipeline with examples of command usage for [Oxford Nanopore Technology long-reads](https://github.com/genomicsITER/monkeypox/blob/main/codes/code_ONT-and-HybridAssembly_pipeline.md).

<hr>

<a name="List-of-software"></a>
**List of bioinformatic software used in our pipelines**
<ul>
  <li>Conda manual for installation of numerous open-source tools used in these pipelines:<a href="https://docs.conda.io/en/latest/">Conda documentation</a></li>
  <li>Programming environment of general purpose: <a href="https://www.r-project.org/">R v.4.1.3</a></li>
  <li>Quality Control of Illumina reads: <a href="https://www.bioinformatics.babraham.ac.uk/projects/fastqc/">FastQC v0.11.9</a></li>
  <li>Adapter trimming: <a href="https://github.com/OpenGene/fastp">fastp v0.23.2</a></li>
  <li>Remove Human mapping-reads from your FASTQ files: <a href="https://ccb.jhu.edu/software/kraken2/">Kraken2 v.2.1.2</a>. If you have issues when downloading the database indexes, try this <a href="https://benlangmead.github.io/aws-indexes/k2" >alternative site</a> from <a href="https://github.com/BenLangmead" >BenLangmead</a>.</li>
  <li>Visualization of Kraken2 reports: <a href="https://ccb.jhu.edu/software/pavian/">Pavian v.1.0</a></li>
  <li>Assemble of Illumina short-reads: <a href="https://github.com/rrwick/Unicycler">Unicycler v0.5.0</a></li>
  <li>Benchmarking and quality control of assemblies: <a href="http://quast.sourceforge.net/">QUAST v.5.0.2</a></li>
  <li>CLI tool to search in nucleotide databases using a nucleotide query: <a href="https://blast.ncbi.nlm.nih.gov/doc/blast-help/">BLAST+ v.2.12.0+</a></li>
  <li>Mapping of short-reads: <a href="https://github.com/lh3/bwa/">BWA v.0.7.17-r1188</a></li>
  <li>Get mapping statistics, manipulate BAM files, and generate mpileups for FASTA consensus: <a href="https://github.com/samtools/samtools">SAMtools v.1.6</a></li>
  <li>Compute the depth of coverage and other statistics: <a href="https://github.com/brentp/mosdepth/">Mosdepth v.0.3.3</a></li>
  <li>Perform the variant calling and consensus: <a href="https://github.com/andersen-lab/ivar/">iVar v.1.3.1</a></li>
  <li>Multiple Sample Alignment: <a href="https://mafft.cbrc.jp/alignment/server/">MAFFT v.7.505]</a></li>
  <li>Phylogenomic inference and tree computing: <a href="http://www.iqtree.org/">IQ-TREE v.2.2.0.3</a></li>
  <li>Framework for analyses and visualization of pathogen genome data (Nextstraing-monkeypox in this case): <a href="https://github.com/nextstrain/monkeypox">Nextstrain</a></li>
  <li>Visualization of phylogenetic trees: <a href="http://tree.bio.ed.ac.uk/software/figtree/">Figtree</a></li>
  <li>Visualization of phylogenetic trees: <a href="https://bioconductor.org/packages/release/bioc/html/ggtree.html/">ggtree 3.15</a></li>
  <li>Annotation of genomes: <a href="https://pcingola.github.io/SnpEff/">SnpEff v.5.1d</a></li>
</ul>

<hr>

<a name="Useful-Files"></a>
**Useful files for the pipelines**

<ul>
  <li>FASTA file (<i>'multiMPXV01.fasta.zip'</i>) with multiple sequences of MPXV from NCBI GenBank to use used in the Multiple Sample Aligment step with MAFFT or Nextstrain-monkeypox, available <a href="https://github.com/genomicsITER/monkeypox/blob/main/files/multiMPXV01.fasta.zip">here</a> (last update: June 16, 2022)</a></li>
  <li>Metadata file (TSV format) to use with a Nextstrain-monkeypox local instance, available <a href="https://github.com/genomicsITER/monkeypox/blob/main/files/nextstrain_monkeypox_hmpxv1_metadata_processed_filtered.tsv">here</a> (last update: June 23, 2022)</a></li>
</ul>

 
<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 3 ------------------ -->

<a name="Sequences"></a>
## Sequences ##

> Consensus FASTA file obtained from a hybrid *de novo* Illumina-Nanopore based assembly and [MT903344.1](https://www.ncbi.nlm.nih.gov/nuccore/MT903344.1). See [Virological post for more details](https://virological.org/)

NCBI GenBank Accession: ON782054. Sequence available as [ MPXV/Spain/HUNSC_ITER_0001a/2022](https://www.ncbi.nlm.nih.gov/nuccore/ON782054)


> Consensus FASTA file obtained from Illumina short-reads mapping to [MT903344.1](https://www.ncbi.nlm.nih.gov/nuccore/MT903344.1). See [Virological post for more details](https://virological.org/)

NCBI GenBank Accession: ON782055. Sequence available as [ MPXV/Spain/HUNSC_ITER_0001b/2022](https://www.ncbi.nlm.nih.gov/nuccore/ON782055)

> For the published paper (<a href="#How-to-cite">see below</a>), we have sequenced more samples. Their sequences are publicly available as follows:
- MPXV sequences of MPXV01, MPXV05, MPXV06 and MPXV07 samples obtained from the Illumina-only consensus approach have been released in the NCBI GenBank with accessions [ON782054](https://www.ncbi.nlm.nih.gov/nuccore/ON782054), [OQ581847](https://www.ncbi.nlm.nih.gov/nuccore/OQ581847), [OQ581848](https://www.ncbi.nlm.nih.gov/nuccore/OQ581848), and [OQ581849](https://www.ncbi.nlm.nih.gov/nuccore/OQ581849), respectively.
- Hybrid de novo assemblies of MPXV01, MPXV05, MPXV06 and MPXV07 samples have also been released with accessions [ON782055](https://www.ncbi.nlm.nih.gov/nuccore/ON782055), [OQ581850](https://www.ncbi.nlm.nih.gov/nuccore/OQ581850), [OQ581851](https://www.ncbi.nlm.nih.gov/nuccore/OQ581851), and [OQ581852](https://www.ncbi.nlm.nih.gov/nuccore/OQ581852), respectively.




<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 4 ------------------ -->

<a name="How-to-GenBank"></a>
## How to download sequences and metadata from GenBank ##

> Manual download

<ol>
<li>Browse to <a href="https://www.ncbi.nlm.nih.gov/genbank/">GenBank</a>.</li>
<li>Select '<i>Nucleotide</i>' from the combo box.</li>
<li>Fill in the accession code of the sequence you want to download (i.e. ON782054) or just write the name of the species (i.e. Monkeypox, and then clic on a certain accession code you are interested in).</li>
<li>Click on '<i>FASTA</i>' link</li>
<li>Click on '<i>Send to</i>' on the upper right part of the screen.</li>
<li>Select the option '<i>file</i>'.</li>
<li>Select '<i>FASTA</i>' as download format.</li>
<li>Click on '<i>Generate</i>' button.</li>
</ol>

> Programmatically download

<a href="https://github.com/genomicsITER/monkeypox/blob/main/codes/code_retrieve-seqs-from-GenBank.md"><img src="https://github.com/genomicsITER/monkeypox/blob/main/images/Code-Window-icon.png" width="32px" /></a>  We provide a full Python code to retrieve all sequences larger than 190,000 bases from GenBank as example. [See the code](https://github.com/genomicsITER/monkeypox/blob/main/codes/code_retrieve-seqs-from-GenBank.md).



<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>

<hr>
<!-- ------------------ SECTION 5 ------------------ -->

<a name="DNA-depletion"></a>
## Enrichment of viral DNA by means of Human & Bacterial DNA depletion ##

<ul>
<li><a href="https://international.neb.com/products/e2612-nebnext-microbiome-dna-enrichment-kit#Product%20Information" target="_blank">NEBNext® Microbiome DNA Enrichment Kit</a>. See <a href="https://virological.org/t/monkeypox-virus-genome-sequences-from-multiple-lesions-indicates-co-infection-of-a-uk-returning-traveller/873">this post</a> at Virological.org</li>
<li>See <a href="https://www.medrxiv.org/content/10.1101/2022.07.29.22278145v1">"A new and efficient enrichment method for metagenomic sequencing of monkeypox virus"</a>, which performs host DNA depletion using a saponin/NaCl combination treatment and DNase.</li>
</ul>

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>

<hr>
<!-- ------------------ SECTION 6 ------------------ -->

<a name="Other-repos"></a>
## Other useful repositories with resources to study MPXV ##

> Kudos to all research teams behind the scenes in all these repositories:
> 
<ul>
  <li><a href="https://www.who.int/publications/i/item/WHO-MPX-laboratory-2022.1">WHO Laboratory testing for the monkeypox virus: Interim guidance (and Corrigendums), 23 May 2022</a></li>
  <li>European Centre for Disease Prevention and Control (ECDC), <a href="https://www.ecdc.europa.eu/en/monkeypox">Monkeypox resource center</a></li>
  <li>Joint ECDC-WHO Regional Office for Europe <a href="https://monkeypoxreport.ecdc.europa.eu/">Monkeypox Surveillance Bulletin</a></li>
  <li><a href="https://virological.org/c/monkeypox">Virological.org posts on MPXV</a></li>
  <li><a href="https://github.com/CADDE-CENTRE/Monkeypox">CADDE-CENTRE GitHub repository for MPXV</a></li>  
  <li><a href="https://github.com/Mike-Honey/mpx-22">Mike Honey GitHub repository for MPXV</a></li>
  <li><a href="https://mpox.genspectrum.org/explore">Mpox-Spectrum from the Computational Evolution group of ETH Zürich in Switzerland</a></li>
  <li><a href="https://github.com/globaldothealth/monkeypox">Global.health, geospatial data visualisations to explore MPXV GitHub repository</a> and <a href="https://map.monkeypox.global.health/country">visualization</a></li>
  <li><a href="https://ourworldindata.org/monkeypox">Our World in Data for MPXV</a></li>
  <li><a href="https://github.com/nextstrain/monkeypox">Nextstraing build for MPXV in GitHub</a> and <a href="https://nextstrain.org/monkeypox/hmpxv1">visualization</a></li>
  <li><a href="https://www.finddx.org/mpx-test-directory/">FIND offers a searchable directory of monkeypox tests</a></li>
</ul>

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 7 ------------------ -->

<a name="References"></a>
## References ##

> Published papers

Alcolea-Medina, Adela and Charalampous, Themoula and Snell, Luke B. and Aydin, Alp and Alder, Christopher and Maloney, Gillian and Bryan, Lisa and Nebbia, Gaia and Douthwaite, Sam and Neil, Stuart and Cliff, Penelope and O'Grady, Justin and Batra, Rahul and Wilks, Mark and O'Hara, Geraldine and Edgeworth, Jonathan, Novel, Rapid Metagenomic Method to Detect Emerging Viral Pathogens Applied to Human Monkeypox Infections (June 9, 2022). Available at SSRN: https://ssrn.com/abstract=4132526 or http://dx.doi.org/10.2139/ssrn.4132526

Berthet N, Descorps-Declère S, Besombes C, et al. Genomic history of human monkey pox infections in the Central African Republic between 2001 and 2018. Sci Rep. 2021;11(1):13085. Published 2021 Jun 22. doi: https://doi.org/10.1038/s41598-021-92315-8

Cervantes-Gracia K, Gramalla-Schmitz A, Weischedel J, Chahwan R. APOBECs orchestrate genomic and epigenomic editing across health and disease. Trends Genet. 2021;37(11):1028-1043. doi: https://doi.org/10.1016/j.tig.2021.07.003

Cohen J. Global outbreak puts spotlight on neglected virus. Science. 2022;376(6597):1032-1033. doi:10.1126/science.add2701

Cohen-Gihon I, Israeli O, Shifman O, et al. Identification and Whole-Genome Sequencing of a Monkeypox Virus Strain Isolated in Israel. Microbiol Resour Announc. 2020;9(10):e01524-19. Published 2020 Mar 5. doi: https://doi.org/10.1128/MRA.01524-19

Erez N, Achdout H, Milrot E, et al. Diagnosis of Imported Monkeypox, Israel, 2018. Emerg Infect Dis. 2019;25(5):980-983. doi:10.3201/eid2505.190076

Faye O, Pratt CB, Faye M, et al. Genomic characterisation of human monkeypox virus in Nigeria [published correction appears in Lancet Infect Dis. 2018 Mar;18(3):244]. Lancet Infect Dis. 2018;18(3):246. doi: https://doi.org/10.1016/S1473-3099(18)30043-4

Iizuka I, Saijo M, Shiota T, et al. Loop-mediated isothermal amplification-based diagnostic assay for monkeypox virus infections. J Med Virol. 2009;81(6):1102-1108. doi: https://doi.org/10.1002/jmv.21494

Kraemer MUG, Tegally H, Pigott DM, et al. Tracking the 2022 monkeypox outbreak with epidemiological data in real-time [published online ahead of print, 2022 Jun 8]. Lancet Infect Dis. 2022;S1473-3099(22)00359-0. doi: https://doi.org/10.1016/S1473-3099(22)00359-0

Kugelman JR, Johnston SC, Mulembakani PM, et al. Genomic variability of monkeypox virus among humans, Democratic Republic of the Congo. Emerg Infect Dis. 2014;20(2):232-239. doi: https://doi.org/10.3201/eid2002.130118

Kulesh DA, Loveless BM, Norwood D, et al. Monkeypox virus detection in rodents using real-time 3'-minor groove binder TaqMan assays on the Roche LightCycler. Lab Invest. 2004;84(9):1200-1208. doi: https://doi.org/10.1038/labinvest.3700143

Li D, Wilkins K, McCollum AM, et al. Evaluation of the GeneXpert for Human Monkeypox Diagnosis. Am J Trop Med Hyg. 2017;96(2):405-410. doi:10.4269/ajtmh.16-0567

Li Y, Olson VA, Laue T, Laker MT, Damon IK. Detection of monkeypox virus with real-time PCR assays. J Clin Virol. 2006;36(3):194-203. doi: https://doi.org/10.1016/j.jcv.2006.03.012

Li Y, Zhao H, Wilkins K, Hughes C, Damon IK. Real-time PCR assays for the specific detection of monkeypox virus West African and Congo Basin strain DNA. J Virol Methods. 2010;169(1):223-227. doi: https://doi.org/10.1016/j.jviromet.2010.07.012

Luciani L, Inchauste L, Ferraris O, et al. A novel and sensitive real-time PCR system for universal detection of poxviruses [published correction appears in Sci Rep. 2022 Apr 8;12(1):5961]. Sci Rep. 2021;11(1):1798. Published 2021 Jan 19. doi: https://doi.org/10.1038/s41598-021-81376-4

Maksyutov RA, Gavrilova EV, Shchelkunov SN. Species-specific differentiation of variola, monkeypox, and varicella-zoster viruses by multiplex real-time PCR assay. J Virol Methods. 2016;236:215-220. doi: https://doi.org/10.1016/j.jviromet.2016.07.024

Mucker EM, Hartmann C, Hering D, et al. Validation of a pan-orthopox real-time PCR assay for the detection and quantification of viral genomes from nonhuman primate blood. Virol J. 2017;14(1):210. Published 2017 Nov 3. doi: https://doi.org/10.1186/s12985-017-0880-8

Patrono LV, Pléh K, Samuni L, et al. Monkeypox virus emergence in wild chimpanzees reveals distinct clinical outcomes and viral diversity. Nat Microbiol. 2020;5(7):955-965. doi: https://doi.org/10.1038/s41564-020-0706-0

Pecori R, Di Giorgio S, Paulo Lorenzo J, Nina Papavasiliou F. Functions and consequences of AID/APOBEC-mediated DNA and RNA deamination [published online ahead of print, 2022 Mar 7]. Nat Rev Genet. 2022;1-14. doi: https://doi.org/10.1038/s41576-022-00459-8

Seang, S., Burrel, S., Todesco, E., Leducq, V., Monsel, G., Le Pluart, D., Cordevant, C., Pourcher, V., & Palich, R. (2022). Evidence of human-to-dog transmission of monkeypox virus. Lancet (London, England), S0140-6736(22)01487-8. Advance online publication. doi: https://doi.org/10.1016/S0140-6736(22)01487-8

Shchelkunov SN, Shcherbakov DN, Maksyutov RA, Gavrilova EV. Species-specific identification of variola, monkeypox, cowpox, and vaccinia viruses by multiplex real-time PCR assay. J Virol Methods. 2011;175(2):163-169. doi: https://doi.org/10.1016/j.jviromet.2011.05.002

Tumewu J, Wardiana M, Ervianty E, et al. An adult patient with suspected of monkeypox infection differential diagnosed to chickenpox. Infect Dis Rep. 2020;12(Suppl 1):8724. Published 2020 Jul 6. doi: https://doi.org/10.4081/idr.2020.8724

Yong SEF, Ng OT, Ho ZJM, et al. Imported Monkeypox, Singapore. Emerg Infect Dis. 2020;26(8):1826-1830. doi:10.3201/eid2608.191387

Zhao K, Wohlhueter RM, Li Y. Finishing monkeypox genomes from short reads: assembly analysis and a neural network method. BMC Genomics. 2016;17 Suppl 5(Suppl 5):497. Published 2016 Aug 31. doi: https://doi.org/10.1186/s12864-016-2826-8



> Preprint papers

A new and efficient enrichment method for metagenomic sequencing of monkeypox virus
Pablo Aja-Macaya, Soraya Rumbo-Feal, Margarita Poza, Angelina Cañizares, Juan A. Vallejo and Germán Bou
medRxiv 2022.07.29.22278145v1; doi: https://doi.org/10.1101/2022.07.29.22278145

Enhanced surveillance of monkeypox in Bas-Uélé, Democratic Republic of Congo: the limitations of symptom-based case definitions
Gaspard Mande, Innocent Akonda, Anja De Weggheleire, Isabel Brosius, Laurens Liesenborghs, Emmanuel Bottieau, Noam Ross, Guy -Crispin Gembu, Robert Colebunders, Erik Verheyen, Ngonda Dauly, Herwig Leirs, Anne Laudisoit
medRxiv 2022.06.03.22275815; doi: https://doi.org/10.1101/2022.06.03.22275815



<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 8 ------------------ -->

<a name="Acknowledgements"></a>
## Acknowledgements ##

This study has been funded by Cabildo Insular de Tenerife (CGIEU0000219140 and "_Apuestas científicas del ITER para colaborar en la lucha contra la COVID-19_"), Instituto de Salud Carlos III (FI18/00230) cofunded by European Union (ERDF) "_A way of making Europe_", and by the agreement with Instituto Tecnológico y de Energías Renovables (ITER) to strengthen scientific and technological education, training, research, development and innovation in Genomics, Personalized Medicine and Biotechnology (OA17/008).

We acknowledge in [Table 1 (EXCEL file)](https://github.com/genomicsITER/monkeypox/blob/main/tables/table1.xlsx) the researchers and their institutions who released the MPXV sequences through NCBI GenBank that are being used in our studies. 

We also thank the authors, the laboratories that originated and submitted the genetic sequences and the metadata for sharing their work, as shown on Nextstrain, and:
<ul>
  <li>Hadfield <i>et al</i>, Nextstrain: real-time tracking of pathogen evolution, Bioinformatics (2018).</li>
  <li>Sagulenko <i>et al</i>, TreeTime: Maximum-likelihood phylodynamic analysis, Virus Evolution (2017).</li>
</ul>

We would like to acknowledge the contributions of several researchers and laboratories who share their preliminary results through the [Virological](https://virological.org/) website.

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 9 ------------------ -->

<a name="License and Attribution"></a>
## License and Attribution ##

This repository and data exports are released under the CC BY 4.0 license. Please acknowledge the authors, the originating and submitting laboratories for the genetic sequences and metadata, and the open source software used in this work (third-party copyrights and licenses may apply).

Please cite this repository as: _"Influenza repository of the Reference Laboratory for Epidemiological Surveillance of Pathogens in the Canary Islands (accessed on YYYY-MM-DD)"_. And do not forget to <a href="#How-to-cite">cite the paper</a> (see the section "How to cite" below) when it becomes available.

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 10 ------------------ -->

<a name="Participating"></a>
## Participating ##

> Want to share your relevant links? Place a Direct Message to @labcflores, @adrmunozb or @resocios on Twitter (see below).

 <p align="left">
  <a href="https://www.iter.es/areas/area-genomica/" title="Contact us at the Genomics Division of the Institute of Technology and Renewable Energy (ITER), Tenerife, Canary Islands, Spain">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/ITER_logo.png" width="30%" /> 
  </a>
</p>

By AMB <a href="https://twitter.com/adrmunozb" title="Follow to @resocios on Twitter" >@adrmunozb <img src="https://github.com/genomicsITER/influenza/blob/main/images/Twitter_Social_Icon_Circle_Color.png" width="32px" /></a> and JMLS <a href="https://twitter.com/resocios" title="Follow to @resocios on Twitter" >@resocios <img src="https://github.com/genomicsITER/influenza/blob/main/images/Twitter_Social_Icon_Circle_Color.png" width="32px" /></a>

Follow us on Twitter <a href="https://twitter.com/labcflores" title="Follow to @labcflores on Twitter" > @labcflores<img src="https://github.com/genomicsITER/influenza/blob/main/images/Twitter_Social_Icon_Circle_Color.png" width="32px" /></a>

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 11 ------------------ -->

<a name="How-to-cite"></a>
## How to cite this work ##

> This work has not been publised yet. See 'License and Attribution' section to cite this repository.

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 12 ------------------ -->

<a name="Update logs"></a>
## Update logs ##

> July 26, 2023. Created the private version of this repository. Enjoy the reading! ;=)

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>
