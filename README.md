## android-ci-cd
***

Fluxo de trabalho que irá automaticamente construir e carregar um APK Android. \
O fluxo de trabalho usa as seguintes etapas: 

Checkout do código do repositório GitHub. \
Configurar o ambiente Java JDK. \
Construa o APK Android usando Gradle. \
Carregue o APK para artefatos do GitHub Actions. 

#### Aqui estão alguns detalhes adicionais: 

Use a ação checkout para verificar o código do repositório GitHub. \
Use a ação setup-java para configurar o ambiente Java JDK. \
Use a ação gradlew para construir o APK Android. \
Use a ação upload-artifact para carregar o APK para artefatos do GitHub Actions. 
