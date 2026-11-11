-- Projeto: Modelo de banco de dados - Professor e Curso
-- SGBD: MySQL
-- Gerado a partir do modelo XML do DBDesigner enviado.

CREATE DATABASE IF NOT EXISTS bd_aula_24_10_26
    CHARACTER SET utf8mb4
    COLLATE utf8mb4_unicode_ci;

USE bd_aula_24_10_26;

-- Tabela de professores
CREATE TABLE IF NOT EXISTS professor (
    idprofessor INT NOT NULL AUTO_INCREMENT,
    nome VARCHAR(255) NULL,
    cidade VARCHAR(255) NULL,
    estado VARCHAR(2) NULL,
    CEP VARCHAR(9) NULL,
    telefone VARCHAR(255) NULL,
    email VARCHAR(255) NULL,
    status INT NULL,
    PRIMARY KEY (idprofessor)
) ENGINE=InnoDB;

-- Tabela de cursos
CREATE TABLE IF NOT EXISTS Curso (
    idCurso INT NOT NULL AUTO_INCREMENT,
    professor_idprofessor INT NOT NULL,
    nome VARCHAR(255) NULL,
    Data_inicio DATE NULL,
    Data_termino DATE NULL,
    Status_2 VARCHAR(255) NULL,
    PRIMARY KEY (idCurso),
    INDEX idx_curso_professor (professor_idprofessor),
    CONSTRAINT fk_curso_professor
        FOREIGN KEY (professor_idprofessor)
        REFERENCES professor (idprofessor)
) ENGINE=InnoDB;
