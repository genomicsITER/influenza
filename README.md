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
 <li><a href="https://www.iter.es/areas/genomics/?lang=en">Genomics Division, Instituto Tecnológico y de Energías Renovables</a>, 38600 Santa Cruz de Tenerife, Spain.</li>
</ul>

<hr>
<!-- ------------------ SECTION ------------------ -->

# Table of contents #
<ul>
  <li><a href="#Virological-posts">Virological post: A draft of the first Influenza genomes from the Canary Islands, Spain, 2022-2023</a></li>
  <li><a href="#Protocols">Protocols for library preparation and sequencing of Influenza viral genomes</a></li>
      <ul>
          <li><a href="#PCR-primers">PCR-prinmers</a></li>
          <li><a href="#Illumina-protocol">Illumina-based protocol</a></li>
          <li><a href="#ONT-protocol">ONT-based protocol</a></li>
      </ul>
 <li><a href="#Bioinformatic pipelines">Bioinformatic pipelines</a></li>
      <ul>
           <li><a href="#Code-Illumina">Code for Illumina short-reads processing</a></li>
           <li><a href="#Code-ONT">Code for Nanopore long-reads processing and hybrid <i>de novo</i> assemby</a></li>
           <li><a href="#List-of-software">List of bioinformatic software used in our pipelines</a></li>
           <li><a href="#Useful-Files">Useful files for the pipelines</a></li>
      </ul>
  <li><a href="#Sequences">Sequences</a></li>
  <!-- 
  <li><a href="#How-to-GenBank">How to download sequences and metadata from GenBank</a></li> 
  <li><a href="#DNA-depletion">Enrichment of viral DNA by means of Human & Bacterial DNA depletion</a></li>  
  <li><a href="#Other-repos">Other useful repositories with resources to study MPXV</a></li> -->
  <li><a href="#References">References</a></li>
  <li><a href="#Acknowledgements">Acknowledgements</a></li>
  <li><a href="#License and Attribution">License and Attribution</a></li>
  <li><a href="#Participating">Participating</a></li>
  <li><a href="#How-to-cite">How to cite this work</a></li>
  <li><a href="#Update logs">Update logs</a></li>
</ul>

<hr>
<!-- ------------------ SECTION 1 ------------------ -->

<a name="Virological-posts"></a>
## Virological post: A draft of the first Influenza genomes from the Canary Islands, Spain, 2022-2023 ##

A technical post with the draft of the first Influenza genomes from the Canary Islands, Spain, will be shared through Virological shortly. Keep reading! [Here.](https://virological.org/)

The first genome sequences of Influenza virus A/H1N1 and A/H3N2 described by us in Virological are phylogenetically related to the multiple viral genomes deposited in NCBI GenBank that correspond to the past 2022-2023 seasonal flu wave in the Northern hemisphere, as shown in Figures 1 and 2.

<p align="center">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/figures/Tree_Influenza_A-H1N1_CanaryIslands_Spain.png" width="auto" />
  </a>
</p>

**Figure 1**. A phylogenetic tree depicting the position of the genome draft of Influenza A/H1N1 isolated in the period November-December 2022, from patients from the Canary Islands along with NCBI GenBank publicly available sequences as computed by <a href="https://clades.nextstrain.org/">Nextstrain</a> using the HA gene and Influenza A H1N1pdm HA [<a href="https://www.ncbi.nlm.nih.gov/nuccore/CY163680">A/California/07/2009 (CY121680)</a>] as reference.


<p align="center">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/figures/Tree_Influenza_A-H3N2_CanaryIslands_Spain.png" width="auto" />
  </a>
</p>

**Figure 2**. A phylogenetic tree depicting the position of the genome draft of Influenza A/H3N2 isolated in the period October-December 2022, from patients from the Canary Islands along with NCBI GenBank publicly available sequences as computed by <a href="https://clades.nextstrain.org/">Nextstrain</a> using the HA gene and Influenza A H3N2 HA [<a href="https://www.ncbi.nlm.nih.gov/nuccore/CY163680">A/Wisconsin/67/2005 (CY163680)</a>] as reference.

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>

<hr>
<!-- ------------------ SECTION 2 ------------------ -->

<a name="Protocols"></a>
## Protocols for library preparation and sequencing of Influenza viral genomes ##

Text here.

Text here.

Text here.

<hr>
          
<a name="PCR-primers"></a>
**PCR primers**

Text here.

<hr>

<a name="Illumina-protocol"></a>
**Illumina-based protocol**

Text here.

<hr>

<a name="ONT-protocol"></a>
**ONT-based protocol**

Text here.

<hr>

<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>

<hr>
<!-- ------------------ SECTION 3 ------------------ -->

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
<!-- ------------------ SECTION 5 ------------------ 

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

<hr> -->
<!-- ------------------ SECTION 6 ------------------ -->

<a name="Other-repos"></a>
## Other useful repositories with resources to study Influenza ##

> Kudos to all research teams behind the scenes in all these repositories:
> 
<ul>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
  <li><a href="">text here</a></li>
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





> Preprint papers





<p align="right">
  <a href="#Influenza" title="Up">
    <img src="https://github.com/genomicsITER/influenza/blob/main/images/home-icon.png" style="float: right; margin: 10px; padding: 2px;" />
  </a>
</p>


<hr>
<!-- ------------------ SECTION 8 ------------------ -->

<a name="Acknowledgements"></a>
## Acknowledgements ##

This study has been funded by Cabildo Insular de Tenerife (CGIEU0000219140 and "_Apuestas científicas del ITER para colaborar en la lucha contra la COVID-19_"), Instituto de Salud Carlos III (FI18/00230) cofunded by European Union (ERDF) "_A way of making Europe_", by the agreement with Instituto Tecnológico y de Energías Renovables (ITER) to strengthen scientific and technological education, training, research, development and innovation in Genomics, Personalized Medicine and Biotechnology (OA17/008); and by the agreement between Consejería de Educación, Universidades, Cultura y Deportes del Gobierno de Canarias y Cabildo Insular de Tenerife, 2022-2025.

We acknowledge the researchers and their institutions who released Influenza sequences through NCBI GenBank, GISAID, and ENA that are being used in our studies. 

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
