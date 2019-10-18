{\rtf1\ansi\ansicpg1252\cocoartf1671\cocoasubrtf200
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 create table aluno (alu_id int not null auto_increment,\
					 alu_username varchar(60) not null,\
                     alu_password varchar(60) not null,\
                     alu_nome varchar(60) not null,\
					 alu_morada varchar(30),\
					 alu_email varchar(30),\
                     alu_numero int not null,\
                     alu_telemovel int not null,\
                     alu_fotografia blob not null, \
					 primary key (alu_id));	\
                     \
create table admin (adm_id int not null auto_increment,\
					 adm_username varchar(60) not null,\
                     adm_password varchar(60) not null,\
                     adm_nome varchar(60) not null,\
					 adm_email varchar(30) not null,\
                     adm_telemovel int,\
                     adm_fotografia blob not null,\
					 primary key (adm_id));	\
                     \
create table docente (doc_id int not null auto_increment,\
					 doc_username varchar(60) not null,\
                     doc_password varchar(60) not null,\
                     doc_nome varchar(60) not null,\
					 doc_email varchar(30) not null,\
                     doc_numero int not null,\
                     doc_telemovel int,\
                     doc_fotografia blob not null,\
					 primary key (doc_id));	\
                     \
create table secretariado (sec_id int not null auto_increment,\
					 sec_username varchar(60) not null,\
                     sec_password varchar(60) not null,\
                     sec_nome varchar(60) not null,\
					 sec_email varchar(30) not null,\
                     sec_numero int not null,\
                     sec_telemovel int,\
                     sec_fotografia blob not null,\
					 primary key (sec_id));	\
                     \
		           \
create table disciplina (dis_id int not null auto_increment,\
						  dis_nome varchar(40) not null,\
					      dis_creditos tinyint not null,\
						   dis_alu_id int not null,\
                          dis_doc_id int not null,\
						  primary key (dis_id, dis_alu_id, dis_doc_id));\
		    \
create table planoestudo (pla_id int not null,\
						  pla_dis_id int not null,\
						   pla_cur_id int not null,\
						   pla_semestre int not null,\
						   primary key (pla_id,pla_dis_id, pla_cur_id));\
                           \
create table curso (cur_id int not null auto_increment,\
						   cur_nome varchar (30) not null,\
						   primary key (cur_id));\
                           \
create table classificacao (cla_id int not null auto_increment,\
						 cla_nota int not null,\
                         cla_semestre int not null,\
                         cla_info varchar (30) not null,\
                         cla_dis_id int not null,\
                         cla_pla_id int not null, \
                         cla_alu_id int not null, \
                         cla_adm_id int not null,\
                         cla_doc_id int not null,\
						 primary key (cla_id, cla_dis_id, cla_pla_id, cla_alu_id, cla_adm_id, cla_doc_id));\
                         \
create table mensalidade (men_id int not null auto_increment,\
						men_info varchar(30) not null,\
                        men_valor int not null,\
						men_alu_id int not null,\
                        men_sec_id int not null,\
						 primary key (men_id, men_alu_id, men_sec_id));\
                         \
                         \
-- Chaves estrangeiras\
alter table disciplina add constraint disciplina_fk_aluno\
            foreign key (dis_alu_id) references aluno(alu_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;\
\
alter table disciplina add constraint disciplina_fk_docente\
            foreign key (dis_doc_id) references docente(doc_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;\
            \
alter table planoestudo add constraint planoestudo_fk_disciplina\
            foreign key (pla_dis_id) references disciplina(dis_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;\
\
alter table planoestudo add constraint planoestudo_fk_curso\
            foreign key (pla_cur_id) references curso(cur_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;           \
                       \
alter table classificacao add constraint classificacao_fk_disciplina\
            foreign key (cla_dis_id) references disciplina(dis_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION; \
            \
alter table classificacao add constraint classificacao_fk_planoestudo\
            foreign key (cla_pla_id) references planoestudo(pla_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION; \
                        \
alter table classificacao add constraint classificacao_fk_aluno\
            foreign key (cla_alu_id) references aluno(alu_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION; \
                                  \
alter table classificacao add constraint classificacao_fk_admin\
            foreign key (cla_adm_id) references admin(adm_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION; \
            \
alter table classificacao add constraint classificacao_fk_docente\
            foreign key (cla_doc_id) references docente(doc_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;   \
            \
alter table mensalidade add constraint mensalidade_fk_aluno\
            foreign key (men_alu_id) references aluno(alu_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;\
            \
alter table mensalidade add constraint mensalidade_fk_secretariado\
            foreign key (men_sec_id) references secretariado(sec_id) \
			ON DELETE NO ACTION ON UPDATE NO ACTION;  \
            \
            \
		\
}