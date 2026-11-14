# configuração

Como configurar variáveis de ambiente e integrações de serviços para o Vinyl.

### Configuração do Ambiente

Crie um arquivo `.env` na raiz do projeto e adicione esta variável:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Obtendo uma chave da API do YouTube

1. Acesse o [Google Cloud Console](https://console.cloud.google.com/) e vá até **APIs e Serviços**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. No menu lateral esquerdo, clique em **Biblioteca**.

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Pesquise por **YouTube Data API v3**, selecione no catálogo e clique em **Ativar**.

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Com a API ativada, vá para **Credenciais** no menu lateral, clique em **+ Criar credenciais** e selecione **Chave de API**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. No painel **Criar chave de API**, configure as opções e clique em **Criar**:
   - **Nome:** Digite um nome identificável (ex: `vinyl-key`).
   - **APIs que podem ser acessadas com esta chave:** Selecione **YouTube Data API v3** nas restrições de API.
   - **Restrições de aplicativo:** Mantenha como **Nenhuma**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Copie a chave de API gerada e atribua a `YOUTUBE_API_KEY` no seu arquivo `.env`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> O Google Cloud oferece uma cota diária gratuita para o YouTube Data API que é mais do que suficiente para desenvolvimento local e uso pessoal.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Anterior: Instalação</strong></a>
</div>

---

*Aviso Legal: Este documento foi traduzido por um processo automatizado interno de IA e pode conter falhas, imprecisões ou erros. A documentação original em inglês deve ser considerada a fonte oficial de referência.*
