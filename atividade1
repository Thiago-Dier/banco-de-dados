create database Biblioteca;
use Biblioteca;

create table Autor
(
	id_autor int primary key not null,
    nome varchar(100) not null,
    nacionalidade varchar(50)
);

create table Livro
(
	id_livro int primary key not null,
    titulo varchar(150) not null,
    ano int,
    editora varchar(80)
);

create table Aluno
(
	id_aluno int primary key not null,
    nome varchar(100) not null,
    email varchar(100) unique,
    curso varchar(50)
);

show tables;

alter table Aluno add telefone int unique;
alter table Livro add isbn int not null;
alter table Livro modify editora varchar(120);
alter table Livro change anoPublicacao ano_publicacao int;
alter table Aluno drop telefone;

alter table Livro add id_autor int;
alter table Livro add foreign key (id_autor) references Livro(id_livro);
alter table Livro modify editora varchar(120) not null;
alter table Livro modify ano_publicacao date;
alter table Livro add email varchar(100) unique;

drop table Aluno;
drop table Livro;
drop database Biblioteca;
