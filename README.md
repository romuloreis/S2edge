
# S2edge - Simple Simulator to Edge

# Papers

**Overview on Edge Computing**

  - [IoT Comic Book](https://drive.google.com/file/d/1ChouVHAa0OxDT1cK3hnuGXK04SC8zkxs/view?usp=sharing)
  - [Survey - Edge](https://drive.google.com/file/d/1Mybe-CyLMRBSJemb9xi7mFPJlqYImTMn/view?usp=sharing)
  - [Artigo SBRC](https://drive.google.com/file/d/1Y4hif0Qc5UIZAsrok2qE9wWHzW9udMki/view?usp=sharing)
  - [Thesis Proposal](https://drive.google.com/file/d/1Y4hif0Qc5UIZAsrok2qE9wWHzW9udMki/view?usp=sharing)
 
 **YAFS**
 
  - [YAFS - Github Repository](https://github.com/acsicuib/YAFS)
  - [Oficial YAFS Paper](https://arxiv.org/abs/1902.01091)
  
  **More articles**
  
    - [Edge/Fog history and real application examples](https://www.microsoft.com/en-us/research/uploads/prod/2018/10/edge-computing-a-historical-perspective-and-direction.pdf)
    - [Survey about fog/edge app placement](https://arxiv.org/abs/1901.05717)

## TO-DO List
  - Upload my code
  - Questions: 
    - Qual o futuro do projeto YAFS? 
    - Pq python 2.7? 
      - As dependencias citadas no git do YAFS (Simpy, Networkx, Numpy, Pandas, tqdm) tem suporte ao python > 3
    - Como fazer o port para python 3+?
      - Foi criada uma seção sobre o port da versão 2 para 3 - Requer bastante trabalho braçal


## Scenario Description
## Parameters



```
Entity - Dispositivos físicos.

entity_name   = {"id": 0, "model": "cloud","mytag":"cloud", "IPT": 5000 * 10 ^ 6, "RAM": 40000,"COST": 3,"WATT":20.0}

int id
int type
position_x
position_y
region
cpu
ram
storage
bw
boolean idle
vm_list
cost_per_second
costPerMem
costPerStorage
costPerBw
```

```
Link Enlaces

    link_name = {"s": 0, "d": 1, "BW": 1, "PR": 10}

type
max_bw
cur_bw
latency
weight
```


```
Instância de serviço

id
type
service_id
cpu
ram
storage
bw
idle
userId
currentAllocatedStorageSize
currentAllocatedRam
currentAllocatedBw
mapped
```

```
Entidade consumidora

id
position_x
position_y
type
service_list
```


## List of commands to install YAFS

```bash
sudo apt-get install python-pip

sudo apt-get install python2.7

git clone https://github.com/acsicuib/YAFS

cd YAFS

sudo python setup.py install

sudo python -m pip install -U matplotlib

sudo apt-get install python-tk

#Maybe you'll need to install network x
sudo pip install networkx
```


## Porting Python 2 to 3

 - [documento oficial](https://docs.python.org/3/howto/pyporting.html)
 - [texto sobre pq devemos migrar](http://blog.aprendapython.com.br/articles/python2-ou-3-1fr71/)
 - [outro texto com motivos](http://www.zeletron.com.br/2013/03/portando-para-o-python-3.html)
 - [Relato de uma migração](https://www.agatetepe.com.br/licoes-aprendidas-da-migracao-para-o-python-3/)
 - [Diferença entre versões](https://blog.caelum.com.br/quais-as-diferencas-entre-python-2-e-python-3/)
 - [Cheat Sheet](http://python-future.org/compatible_idioms.html)
 

