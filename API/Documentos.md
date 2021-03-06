**[Integra��o via API](Guideline.md) - Documentos**

**A��es dispon�veis:**
- [Capturar](#capturar)
  - Capturar Documentos C�pia, Nato-digital ou digitalizado
  - Capturar Documentos que possuem Assinatura Digital
  - Capturar Documentos fazendo a Assinatura Eletr�nica do E-Docs
  - Capturar um Documento para ser Assinado Eletronicamente via E-Docs
  - Assinar um Documento que est� em fase de assinatura
  - Recusar um Documento que est� em fase de assinatura
  - Bloquear um Documento que est� em fase de assinatura
  - Desbloquear um Documento que est� em fase de assinatura
- [Consultar](#consultar)

### Capturar
A captura do Documento � a forma de institucionaliz�-lo e fazer com que ele possa ser utilizado dentro do E-Docs.

A documenta��o deste m�todo pode ser vista [aqui](https://api.e-docs.es.gov.br/swagger/index.html#/Documentos/Documentos_Post).

O Access Token obtido atrav�s da **Autentica��o de Usu�rio** no Acesso Cidad�o utilizando o scope 'api-sigades-documento' � requerido no cabe�alho das requisi��es aos endpoints de Captura usando o padr�o Bearer Token. [Especifica��o de uso do Bearer Token](https://tools.ietf.org/html/rfc6750#page-5)

Para melhor entendimento, o Documento pode ser categorizado quando � sua Natureza, Valor Legal e G�nero

Natureza:
- Nato-digital
- Digitalizado

Valor Legal:
- Original. 
- C�pia Autenticada Administrativamente
- C�pia Simples

G�nero:
- Textual
- �udio
- V�deo

### Consultar
Ap�s um Documento ser capturado ele poder� ser consultado.

A documenta��o deste m�todo pode ser vista [aqui](https://api.e-docs.es.gov.br/swagger/index.html#/Documentos/Documentos_Get).

O Access Token obtido atrav�s da autentica��o no Acesso Cidad�o utilizando o scope 'api-sigades-consultar' ou 'api-sigades-documento' � requerido no cabe�alho das requisi��es aos endpoints de Consulta usando o padr�o Bearer Token. [Especifica��o de uso do Bearer Token](https://tools.ietf.org/html/rfc6750#page-5)