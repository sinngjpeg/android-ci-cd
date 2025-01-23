# 🤖 Android CI/CD Workflow

Este repositório contém um **fluxo de trabalho automatizado** para construir e carregar um APK Android utilizando **GitHub Actions**. 🚀

## 🛠️ **Visão Geral do Fluxo de Trabalho**

O fluxo de trabalho realiza as seguintes etapas de forma automática:

1. ✅ **Checkout do Código:** Faz o checkout do repositório no GitHub.
2. ☕ **Configuração do Ambiente Java JDK:** Configura o ambiente necessário para a construção do APK.
3. 🏗️ **Construção do APK:** Utiliza o Gradle para compilar o projeto Android e gerar o APK.
4. 📦 **Upload do APK:** Carrega o APK gerado como artefato nos GitHub Actions.

---

## 🔍 **Detalhes das Etapas**

### 1️⃣ **Checkout do Código**
- Utiliza a ação `actions/checkout` para clonar o código do repositório no ambiente de execução.

### 2️⃣ **Configuração do Ambiente Java JDK**
- Usa a ação `actions/setup-java` para configurar a versão necessária do Java Development Kit (JDK), essencial para compilar projetos Android.

### 3️⃣ **Construção do APK**
- Utiliza o comando `./gradlew assembleRelease` para construir o APK na variante de release.
- Gradle é configurado automaticamente para gerenciar dependências e compilar o código.

### 4️⃣ **Upload do APK**
- A ação `actions/upload-artifact` é utilizada para armazenar o APK gerado como um artefato nos GitHub Actions, permitindo que ele seja baixado posteriormente.

---

## 📋 **Como Funciona**

1. O fluxo de trabalho é acionado automaticamente quando há um evento configurado no repositório (por exemplo, push ou pull request).
2. Ele executa as etapas descritas acima em sequência.
3. Após a execução, o APK gerado estará disponível como artefato no painel dos GitHub Actions.

---

## ⚙️ **Benefícios**

- 📈 **Automação Total:** Reduz erros manuais e acelera o processo de build.
- 🕒 **Economia de Tempo:** O APK é gerado automaticamente após cada alteração no código.
- 📦 **Artefatos Centralizados:** O APK fica armazenado diretamente nos GitHub Actions, facilitando o acesso.

---

💡 *Dica:* Este fluxo de trabalho pode ser facilmente adaptado para incluir etapas adicionais, como testes automatizados ou publicação em lojas de aplicativos! 🚀
