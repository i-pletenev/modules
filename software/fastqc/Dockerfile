FROM nfcore/base:1.7
LABEL authors="phil.ewels@scilifelab.se" \
    description="Docker image for nf-core modules fastqc"

# foobar
COPY environment.yml /
RUN conda env create -f /environment.yml && conda clean -a
ENV PATH /opt/conda/envs/nf-core-modules-fastqc/bin:$PATH
