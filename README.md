# Spring Cloud Microservices Demo

Este projeto é uma demonstração prática de uma arquitetura de microsserviços utilizando **Java**, **Spring Boot**, e **Spring Cloud**.O sistema implementa conceitos modernos
de autenticação, roteamento, discovery service, e integração entre serviços.

## 🧩 Visão Geral

O sistema é composto por vários microsserviços independentes que se comunicam entre si via HTTP, utilizando o padrão REST e autenticação com JWT.

### Estrutura dos serviços

- **Config Server**: Centraliza a configuração de todos os microsserviços via Git.
- **Eureka Server**: Serviço de registro e descoberta.
- **Zuul Gateway**: Roteador de entrada (API Gateway).
- **Auth Service**: Servidor de autenticação com JWT.
- **User Service**: Gerencia usuários do sistema.
- **Worker Service**: Responsável por trabalhadores e cálculos.
- **Payroll Service**: Integra dados de usuário e trabalhador para cálculo de pagamento.

## 🔐 Autenticação

A autenticação é baseada em **OAuth2** e **JWT**, com a seguinte estrutura:

- **Authorization Server**: emite tokens com base nas credenciais.
- **Resource Servers**: validam o token e fornecem acesso aos recursos.

## ⚙️ Tecnologias utilizadas

- Java 11
- Spring Boot
- Spring Cloud (Config, Eureka, Zuul, OAuth2)
- Docker
- Postman (para testes)
- Git

1. Clone este repositório:
  
   git clone 

2.Inicie os serviços (ordem recomendada):

Config Server

Eureka Server

Zuul Gateway

Auth Service

Outros serviços (User, Worker, Payroll)

3.Teste os endpoints com Postman ou via navegador.
