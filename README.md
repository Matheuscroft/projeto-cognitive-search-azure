### **Azure Cognitive Search: Indexação e Consulta de Dados**  

Esse projeto explora o uso da **Azure AI Search** para indexação e busca de dados utilizando Inteligência Artificial.  

---  

## ⚙️ **Passo a Passo para Configurar a Pesquisa Cognitiva do Azure**  

### **1️⃣ Criar um Serviço de AI Search no Azure**  
1. Acesse o **[Portal do Azure](https://portal.azure.com)** e faça login.  
2. Vá até **"Criar um Recurso"** > **Azure AI Services** > **AI Search**.  
3. Escolha um nome para o serviço e selecione a camada de preços **Básica** (Basic).  
4. Clique em **"Criar"** e aguarde a implantação do serviço.  

---

### **2️⃣ Criar um Serviço de Armazenamento para os Dados**  
1. No Portal do Azure, vá para **"Contas de Armazenamento"** > **"Criar"**.  
2. Escolha a opção de **Redundância LRS** para armazenamento local.  
3. Após a criação, acesse o recurso e vá para **Configurações** > **Configuração**.  
4. Ative a opção **"Permitir acesso anônimo ao Blob"** e clique em **Salvar**.  

---

### **3️⃣ Criar um Container e Enviar Arquivos**  
1. No serviço de armazenamento, vá até **Data Storage** > **Containers**.  
2. Clique em **"+" Criar Container"** e defina o nível de acesso para **Container**.  
3. Clique no container criado e faça **upload dos arquivos** (documentos, PDFs, etc.).  

---

### **4️⃣ Criar um Índice na Pesquisa Cognitiva**  
1. No Portal do Azure, acesse o serviço **Azure AI Search** criado anteriormente.  
2. Vá até **"Data Sources"** e selecione **"Azure Blob Storage"**.  
3. Escolha o container onde os arquivos foram enviados.  
4. Configure as habilidades de IA para **reconhecimento de entidades, tradução e análise de sentimento**.  
5. Execute a indexação e aguarde a finalização do processo.  

---

### **5️⃣ Consultar os Dados Indexados**  
1. No painel da Pesquisa Cognitiva, vá até **"Indexers"** e clique para visualizar os índices criados.  
2. Acesse a aba **"Search Explorer"** e digite uma consulta para buscar informações nos documentos.  
3. É possível usar consultas avançadas, como:  

   ```json
   {
     "search": "hotel",
     "filter": "rating gt 4",
     "select": "title, description, sentiment_score"
   }
   ```  

---

## 🔍 **Insights e Aplicações**  
- **Melhoria na busca de documentos**: Arquivos antes inacessíveis podem ser pesquisados e classificados por relevância.  
- **Integração com chatbots e assistentes virtuais**: Permite a criação de assistentes inteligentes que respondem a perguntas com base nos documentos.  
- **Análise de sentimentos e extração de insights**: Com IA, é possível obter insights sobre avaliações e tendências.  

---

## 📌 **Aprendizados**  
✔️ A importância da **indexação eficiente** para tornar grandes volumes de dados pesquisáveis.  
✔️ Como **habilidades de IA** podem enriquecer os dados e fornecer insights úteis.  
✔️ O poder da **integração entre Azure Storage e AI Search** para organizar e recuperar informações rapidamente.  
