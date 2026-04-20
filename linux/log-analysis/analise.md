# Dia 1 - Análise de Logs

## Objetivo
Identificar IP suspeito em tentativas de login

## Comandos usados
grep "failed" auth.log
grep "failed" auth.log | awk '{print $NF}'
grep "failed" auth.log | awk '{print $NF}' | sort | uniq -c | sort -nr

## Resultado
O IP 185.23.54.1 realizou mais tentativas de login falhas.

## Observação
Esse tipo de análise é comum em SOC para detectar ataques de brute force.
