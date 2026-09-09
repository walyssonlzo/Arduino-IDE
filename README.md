# Projeto_LDR_Arduino

💡 **Controle de LED por LDR com Arduino**

---

## 📄 Descrição do Projeto

Este projeto utiliza a plataforma Arduino para monitorar a intensidade luminosa do ambiente através de um sensor LDR (Resistor Dependente de Luz). Com base nos valores capturados pelo sensor, o sistema processa os dados de entrada e ajusta a saída para acionar o LED (acender/apagar), criando uma resposta automática à variação de iluminação.

---

## 👥 Integrantes da Equipe

- **Letícia Halana** - Instrutora
- **Walysson Henryque** - Aluno
- **Mateus Alves** - Aluno
- **Dabliele** - Aluno
- **Maria Emanuely** - Aluno

---

## 🛠️ Materiais e Componentes Eletrônicos

| Componente | Quantidade | Observação |
|---|---|---|
| Arduino Uno | 1 un. | Ou modelo equivalente |
| Sensor LDR (5mm) | 1 un. | Leitura de luminosidade |
| LED (5mm) | 1 un. | Cor à escolha |
| Resistor de 220 Ω | 1 un. | Redutor de corrente para LED |
| Protoboard | 1 un. | Matriz de contatos |
| Jumpers Macho-Macho | Vários | Conexões do circuito |

---


## 💻 Trecho do Código (Sensores → INPUT)

O trecho de código abaixo exemplifica a lógica do projeto: o sinal analógico lido pelo sensor funciona como entrada (`INPUT`).

```cpp
int LDR = A0; // Entrada do sensor LDR (INPUT)

void setup() {
  pinMode(LDR, INPUT); // Define o pino A0 como Entrada
}