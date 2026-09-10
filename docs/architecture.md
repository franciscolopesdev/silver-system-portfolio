# Arquitetura — Silver System POS

## Objetivo

Documentar as decisões de alto nível que orientaram o projeto sem expor detalhes proprietários.

![Arquitetura](../assets/architecture.svg)

## Banco local centralizado
Todos os aparelhos trabalham sobre o mesmo estado no servidor local, evitando bancos independentes por dispositivo.

## Tempo real
Socket.IO distribui eventos de atualização para manter a operação sincronizada sem refresh manual.

## Impressão operacional
O fluxo foi projetado para direcionar pedidos a setores distintos por ESC/POS.

## Segurança aplicada
Validação de entradas, queries parametrizadas, proteção contra XSS e separação de configurações sensíveis.

## Limites desta documentação

A documentação pública omite deliberadamente código-fonte, credenciais, endpoints internos, esquemas completos de banco, dados de clientes e configurações de infraestrutura.
