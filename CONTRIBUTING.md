# Contribuindo com MadDev

Obrigado por ser parte do projeto da disciplina de **Arquitetura e Desenho de Software**! Este guia descreve como contribuir de forma efetiva e profissional para nosso trabalho.

**Antes de começar:** Por favor discuta sua mudança com o grupo antes de fazer alterações significativas. Use issues, pull requests em draft, ou converse com os responsáveis do repositório.

**Importante:** Temos um código de conduta, siga-o em todas as suas interações com o projeto. Também espera-se que todos sigam boas práticas de arquitetura e desenho de software.

## Reportando Problemas e Questões de Design

Esta seção guia você através do envio de um relatório de problema ou questão relacionada ao design de arquitetura. Seguir estas diretrizes ajuda o time a entender a questão, discutir alternativas e encontrar relatórios relacionados.

Antes de criar um relatório, **verifique a lista de issues** - você pode descobrir que a questão já está em discussão ou foi resolvida. Quando estiver criando um relatório, **inclua o máximo de detalhes possível**. Preencha o template fornecido - as informações nos ajudam a resolver problemas mais rápido.

### Como Enviar um Bom Relatório de Problema?

Problemas são rastreados como [GitHub issues](https://guides.github.com/features/issues/). Crie uma issue no repositório e forneça as seguintes informações:

**Para problemas técnicos:**
- **Use um título claro e descritivo** para identificar o problema
- **Descreva os passos exatos** que reproduzem o problema com o máximo de detalhes possível
- **Forneça exemplos específicos** (links, arquivos, trechos de código, diagramas)
- **Descreva o comportamento observado** e aponte exatamente qual é o problema
- **Explique qual comportamento você esperava ver** e por quê

**Para questões de arquitetura/design:**
- **Título descritivo** da questão ou inconsistência
- **Padrão afetado** (qual componente, camada ou decisão arquitetural)
- **Contexto atual** (como está implementado ou documentado hoje)
- **Impacto** (qual é o problema ou risco)
- **Solução proposta** ou alternativas a considerar
- **Referências** a padrões, boas práticas ou decisões anteriores

**Contexto adicional:**
- **O problema começou recentemente** ou sempre existiu?
- **É reproduzível de forma consistente?** Se não, descreva em quais condições acontece
- **Qual artefato afeta?** (código, documentação, diagrama, etc.)

## Sugerindo Melhorias e Refatorações Arquiteturais

Esta seção guia você através do envio de sugestões de melhoria, incluindo novas features, refatorações arquiteturais e melhorias na documentação.

Antes de criar uma sugestão, **verifique as issues existentes e discussões em aberto**. Quando estiver criando uma sugestão, **inclua justificativa baseada em princípios de arquitetura**. Preencha o template com argumentação clara.

### Como Enviar uma Boa Sugestão de Melhoria?

Sugestões de melhoria são rastreadas como [GitHub issues](https://guides.github.com/features/issues/). Crie uma issue e forneça:

**Para features novas:**
- **Título claro e descritivo** da feature
- **Descrição detalhada** do que está sendo solicitado
- **Casos de uso** que demonstram o valor
- **Comportamento esperado** e critérios de aceitação
- **Impacto na arquitetura** (afeta qual layer, componente, ou padrão?)
- **Exemplos** ou mockups quando relevante

**Para refatorações e melhorias arquiteturais:**
- **Problema identificado** (violação de princípio, design smell, etc.)
- **Padrão/princípio afetado** (SOLID, coesão, acoplamento, etc.)
- **Estado atual** (como funciona/está documentado hoje)
- **Solução proposta** com justificativa técnica
- **Benefícios** (manutenibilidade, escalabilidade, testabilidade, etc.)
- **Impacto** (quais partes do sistema serão afetadas)
- **Referências** a padrões de design ou literaturas sobre o tema

**Geral:**
- **Explique por quê** essa melhoria seria valiosa para o projeto e o grupo

## Processo de Pull Request

O processo descrito aqui tem vários objetivos:

- Corrigir problemas e inconsistências
- Implementar melhorias e novas features
- Manter a qualidade arquitetural do projeto
- Suportar aprendizado colaborativo através de code review

### Passos para Submeter um PR

1. **Crie uma issue** descrevendo o que será feito (ou use uma existente)

2. **Crie uma branch** com nome descritivo vinculado à issue
   ```bash
   git checkout -b feature/ISSUE-#N-descricao-clara
   # ou
   git checkout -b fix/ISSUE-#N-descricao-clara
   ```

3. **Faça suas alterações** em commits pequenos e bem estruturados
   ```bash
   git commit -m "[ISSUE-#N] Descrição clara e objetiva da mudança"
   ```

4. **Atualize artefatos de arquitetura** se necessário
   - Atualize diagramas (UML, BPMN, C4, etc.)
   - Atualize documentação de decisões arquiteturais (ADR)
   - Mantenha o README e documentação sincronizados
   - Inclua explicações de padrões utilizados

5. **Envie um PR em draft** inicialmente, com:
   - Descrição clara do que foi alterado e **por quê**
   - Referência à issue relacionada
   - Justificativa arquitetural se relevante
   - Screenshots ou diagramas atualizados quando aplicável

6. **Solicite revisão** de pelo menos um colega do grupo
   - Procure por alguém com expertise na área afetada
   - Responda perguntas e discuta alternativas

7. **Incorpore feedback** e faça ajustes conforme necessário

8. **Marque como pronto para revisão final** quando sentir-se confiante

9. **Após aprovação**, o PR pode ser feito merge

### Padrões de Qualidade e Arquitetura

**Commits:**
- Mensagens em português, claras e descritivas
- Commits pequenos e focados em uma responsabilidade
- Evite commits genéricos como "corrigir" ou "ajustar"
- Use padrão: `[TIPO] Descrição` (ex: `[FEAT] Implementar autenticação JWT`)

**Código:**
- Mantenha consistência com a estrutura e padrões existentes
- Respeite o estilo de código definido pelo grupo
- Deixe comentários explicativos quando a lógica for complexa
- Aplique padrões de design apropriados
- Considere princípios SOLID

**Documentação:**
- Documentação no código quando necessário (em português)
- Atualize README e documentação de referência
- Para mudanças arquiteturais significativas, crie/atualize um ADR (Architecture Decision Record)
- Mantenha diagramas atualizados

**Validação:**
- Teste suas mudanças antes de enviar
- Verifique se não quebra funcionalidades existentes
- Execute verificações de qualidade/linting se configuradas

### Seu Primeiro Contribution

Não tem certeza por onde começar? Procure por issues marcadas como:

- `good-first-issue` - issues bem contidas e com escopo claro para iniciantes
- `help-wanted` - issues mais envolvidas que procuram volunteers
- `documentation` - melhorias em READMEs, diagramas e artefatos
- `refactoring` - oportunidades para aplicar padrões de design

Além disso:
- Comece revisando issues abertas e veja onde você pode ajudar
- Converse com o time sobre qual seria uma boa primeira tarefa
- Considere começar por melhorias em documentação

## Checklist Antes do Merge

### Issue e Planejamento
- [ ] A issue foi discutida com o time antes de começar?
- [ ] Os requisitos estão claros e aceitos pelo grupo?
- [ ] Há consenso sobre a abordagem arquitetural?

### Código e Arquitetura
- [ ] O código segue padrões e convenções do projeto?
- [ ] Princípios SOLID foram considerados?
- [ ] O design é consistente com a arquitetura existente?
- [ ] Não há violações óbvias de design?

### Documentação
- [ ] Artefatos de arquitetura foram atualizados (diagramas, ADRs)?
- [ ] README e documentação relevante foram atualizados?
- [ ] Código complexo possui comentários explicativos?
- [ ] A mudança foi documentada adequadamente?

### Qualidade
- [ ] As alterações foram testadas localmente?
- [ ] Não há conflitos com a branch principal?
- [ ] Houve revisão técnica de pelo menos um colega?
- [ ] Feedback foi incorporado?

### Processo
- [ ] Você seguiu o código de conduta do projeto?
- [ ] Commits estão bem organizados e com mensagens claras?
- [ ] A descrição do PR explica o quê e o porquê?
- [ ] Referências (issues, padrões, referências) foram incluídas?

## Padrões de Nomenclatura

### Branches
- `feature/ISSUE-#N-nome-da-feature` - Nova funcionalidade
- `fix/ISSUE-#N-descricao-do-problema` - Correção de bug
- `docs/ISSUE-#N-melhorias-documentacao` - Melhorias em documentação
- `refactor/ISSUE-#N-descricao` - Refatoração de código existente

### Commits
- `[FEAT]` - Nova funcionalidade
- `[FIX]` - Correção de bug
- `[DOCS]` - Mudanças em documentação
- `[REFACTOR]` - Refatoração sem mudança de comportamento
- `[STYLE]` - Mudanças de formatação/estilo
- `[TEST]` - Adição ou modificação de testes

Exemplo: `[FEAT] Implementar autenticação OAuth2 com Google`

## Dúvidas?

- Abra uma **issue** para reportar problemas ou sugerir melhorias
- Converse com o time em grupos de comunicação do projeto
- Consulte o professor da disciplina se precisar de orientação