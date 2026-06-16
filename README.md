# Política de Privacidade — Controlo de Acessos

**Última atualização:** 16/06/2026

A presente Política de Privacidade descreve como a aplicação **Controlo de Acessos** recolhe, utiliza e protege os seus dados pessoais. 

Esta aplicação foi desenvolvida para facilitar a gestão e o controlo de acessos remotos a laboratórios e salas institucionais do **Instituto Politécnico de Tomar (IPT)**.

---

## 1. Dados que Recolhemos e Processamos

Para o correto funcionamento da Aplicação, recolhemos e processamos apenas as informações estritamente necessárias para a sua autenticação e para a execução dos comandos de controlo de acessos:

* **Informação de Autenticação:** 
  * E-mail institucional e palavra-passe (para login local).
* **Informação de Utilizador:**
  * Nome do utilizador e Identificador Único de Utilizador (`userId`) fornecidos pela API da instituição após o login.
* **Registos de Acesso (Logs):**
  * Ao solicitar a abertura remota de uma porta, a aplicação envia para a API o seu `userId` e o identificador do laboratório (`labId`). Esta associação é guardada nos servidores da instituição por motivos de segurança e auditoria de acessos.
* **Segurança Local:**
  * Se optar por definir um PIN de acesso rápido na aplicação, este será encriptado e guardado de forma segura no seu dispositivo físico utilizando a biblioteca nativa `androidx.security:security-crypto`. A aplicação não envia o seu PIN para os nossos servidores.

---

## 2. Permissões do Dispositivo

A aplicação solicita apenas as permissões de sistema mínimas necessárias para a sua operação:
* **Acesso à Internet (`INTERNET`):** Necessário para comunicar com a API de Controlo de Acessos e realizar o login.
* **Estado da Rede (`ACCESS_NETWORK_STATE`):** Utilizado para verificar se o dispositivo tem uma ligação ativa à Internet antes de tentar realizar operações.

A Aplicação **não** acede à sua localização por GPS, câmara, galeria de fotos, contactos ou outros dados privados do dispositivo.

---

## 3. Como Utilizamos os Seus Dados

Utilizamos as informações recolhidas exclusivamente para:
1. Autenticar a sua identidade e garantir que tem permissão para aceder à aplicação.
2. Apresentar a lista de laboratórios aos quais tem acesso autorizado.
3. Executar o comando de destrancar portas remotamente a seu pedido.
4. Manter um registo de segurança no servidor para auditar quem acedeu a que salas e a que horas.

---

## 4. Partilha de Dados com Terceiros

Os seus dados são partilhados apenas com os servidores oficiais da instituição e os serviços estritamente necessários para o funcionamento da App:
* **Servidores da Instituição:** Todos os dados de login e comandos de abertura de portas são enviados diretamente para a API de controlo de acessos gerida pelo **IPT**.

**Não vendemos, partilhamos ou divulgamos os seus dados pessoais a redes de publicidade, parceiros comerciais ou quaisquer terceiros para fins lucrativos.**

---

## 5. Segurança dos Dados

A segurança dos seus dados é prioritária. Empregamos medidas técnicas organizativas e protocolos de comunicação seguros (HTTPS/SSL) para proteger os dados em trânsito. Os dados locais confidenciais (como PINs) são protegidos com chaves criptográficas geridas pelo próprio hardware de segurança do dispositivo Android.

---

## 6. Alterações a esta Política de Privacidade

Podemos atualizar a nossa Política de Privacidade periodicamente. Recomendamos que reveja esta página regularmente para tomar conhecimento de quaisquer alterações. As modificações entram em vigor imediatamente após a sua publicação.
