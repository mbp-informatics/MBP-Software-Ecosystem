




flowchart LR
Mosaic[Mosaic Vivarium System]
OTS[MMRRC Order Tracking System]
PTS[MBP Project Tracking System]
IMPC[IMPC / DCC]
Instruments[Phenotyping Instruments]
Robots[Hamilton STAR / Scanner Files]
Cryo[Cryogenic Inventory]

    Pheno[Pheno-LIMS<br/>Phenotyping Workflows]
    Geno[Geno-LIMS<br/>Genotyping Workflows]
    Repro[Repro-LIMS<br/>Mouse Engineering & RT Workflows]

    Mosaic --> Pheno
    Mosaic --> Geno
    Mosaic --> Repro

    Instruments --> Pheno
    Pheno --> IMPC

    Robots --> Geno
    Geno --> Pheno

    OTS --> Repro
    Repro --> PTS
    Repro --> Cryo

    Repro --> Pheno
    Geno --> Repro