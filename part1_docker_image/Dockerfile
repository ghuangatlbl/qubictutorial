FROM nfruitwala/cocotb-verilator:0.4

#clone all repos
RUN git clone https://gitlab.com/lbl-qubic/gateware.git --recursive -b qce24
RUN git clone https://gitlab.com/lbl-qubic/software.git -b sync-refactor
RUN git clone https://gitlab.com/lbl-qubic/distributed_processor.git -b sync-refactor
RUN git clone https://gitlab.com/lbl-qubic/experiments/qubitconfig.git

#pip install them
RUN pip install -e distributed_processor/python
RUN pip install -e software
RUN pip install -e qubitconfig 
RUN pip install pyyaml

#prepare gateware and expose port
RUN cd /gateware/top/zcu216_8_2_tut/; ./configure_build.sh dsp_config.yaml sim
RUN cd /gateware/top/zcu216_8_2_tut/sim; make pre
EXPOSE 9100

WORKDIR /gateware/top/zcu216_8_2_tut/cocotb 
CMD ["make"]
