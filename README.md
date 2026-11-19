
# Aplicativo de Busca de Vagas de Emprego.
PRD Refinado no ChatGPT Web
```
Markdown
# Projeto: MatchCV — Plataforma Inteligente de Matchmaking de Vagas

## 1. Visão geral do produto

Crie uma aplicação web chamada **MatchCV**, uma plataforma inteligente de empregabilidade que utiliza inteligência artificial para conectar candidatos às vagas de emprego mais compatíveis com seus currículos.

O objetivo é simplificar a busca por emprego, permitindo que qualquer pessoa envie seu currículo, receba recomendações personalizadas de oportunidades profissionais e gere versões otimizadas do próprio currículo para cada vaga selecionada.

A experiência deve ser extremamente intuitiva, moderna e acessível, inclusive para pessoas que não possuem conhecimentos técnicos ou experiência com ferramentas de inteligência artificial.

A aplicação deve funcionar sem necessidade de cadastro, login, senha ou autenticação. O usuário deve conseguir acessar a plataforma e utilizar suas funcionalidades imediatamente.

## 2. Objetivos principais

A plataforma deve permitir que o usuário:

1. Envie seu currículo em PDF ou DOCX.
2. Tenha seu currículo analisado automaticamente por inteligência artificial.
3. Identifique suas principais competências, experiências, qualificações e áreas de atuação.
4. Encontre vagas de emprego compatíveis com seu perfil profissional.
5. Visualize um percentual de compatibilidade entre seu currículo e cada vaga.
6. Entenda por que determinada vaga combina com seu perfil.
7. Identifique competências que possui e requisitos que ainda não atende.
8. Selecione uma vaga e gere uma versão personalizada do currículo, otimizada para aquela oportunidade.
9. Baixe o currículo otimizado em PDF e DOCX.
10. Compare o currículo original com a versão adaptada.

## 3. Público-alvo

Pessoas que estão procurando emprego, buscando recolocação profissional ou desejando novas oportunidades de carreira.

A plataforma deve atender tanto profissionais experientes quanto pessoas em início de carreira.

A linguagem utilizada deve ser simples, objetiva, acolhedora e profissional.

## 4. Identidade visual e Design System

Utilize obrigatoriamente **Shadcn/UI como Design System principal**, com componentes consistentes e reutilizáveis.

### Direção visual

Crie uma interface:

- Minimalista e moderna.
- Predominantemente clara (Light Mode).
- Com bastante espaço em branco.
- Com aparência de uma startup SaaS premium.
- Com hierarquia visual bem definida.
- Com tipografia moderna e excelente legibilidade.
- Com elementos visuais discretos e elegantes.

### Paleta de cores

Utilize a seguinte identidade visual:

- Fundo principal: `#FFFFFF`.
- Fundo secundário: `#FFFDF5`.
- Amarelo principal: `#FDE68A`.
- Amarelo de destaque: `#FACC15`.
- Texto principal: `#18181B`.
- Texto secundário: `#71717A`.
- Bordas: `#E4E4E7`.
- Verde para compatibilidade alta: `#16A34A`.
- Laranja para compatibilidade intermediária: `#EA580C`.
- Vermelho para compatibilidade baixa: `#DC2626`.

O amarelo deve ser utilizado em botões principais, destaques, indicadores e pequenos elementos de identidade visual.

Evite grandes áreas com amarelo saturado. Preserve o aspecto clean da aplicação.

### Componentes

Utilize componentes Shadcn/UI, incluindo:

- Button.
- Card.
- Badge.
- Dialog.
- Dropdown Menu.
- Tabs.
- Progress.
- Tooltip.
- Separator.
- Input.
- Textarea.
- Select.
- Skeleton.
- Alert.
- Accordion.
- Sheet.

Utilize ícones Lucide React.

Garanta consistência de espaçamento, bordas, arredondamentos, estados de interação e responsividade.

## 5. Estrutura da aplicação

A aplicação deve possuir as seguintes áreas principais:

### 5.1. Página inicial — Dashboard

A página inicial deve apresentar uma visão geral da experiência.

Elementos:

- Logotipo MatchCV.
- Menu de navegação simples.
- Saudação contextual.
- Título: "Encontre vagas que combinam com você".
- Subtítulo explicando a proposta da plataforma.
- Área de upload do currículo.
- Botão principal: "Analisar meu currículo".
- Área de apresentação das principais funcionalidades.
- Indicadores de vagas encontradas e compatibilidade, quando houver dados disponíveis.

O primeiro contato do usuário deve ser direcionado para o envio do currículo.

Não exija cadastro em nenhuma etapa.

### 5.2. Upload e análise do currículo

Crie uma área de upload intuitiva, com suporte a:

- PDF.
- DOCX.

Permita arrastar e soltar arquivos ou selecioná-los pelo explorador de arquivos.

Após o envio, a inteligência artificial deverá analisar o documento e extrair:

- Nome profissional.
- Cargo atual ou último cargo.
- Resumo profissional.
- Experiências profissionais.
- Empresas e períodos de atuação.
- Formação acadêmica.
- Cursos e certificações.
- Competências técnicas (Hard Skills).
- Competências comportamentais (Soft Skills).
- Idiomas.
- Ferramentas e tecnologias dominadas.
- Áreas de interesse profissional.

Apresente uma tela de processamento com etapas visuais, evitando uma experiência de carregamento genérica.

Após a análise, exiba um perfil profissional estruturado.

O usuário deverá conseguir revisar e corrigir as informações extraídas antes de prosseguir.

Nunca invente informações que não estejam presentes no currículo.

### 5.3. Matchmaking inteligente de vagas

Esta é uma das funcionalidades centrais do produto.

A aplicação deve encontrar oportunidades profissionais compatíveis com o perfil analisado.

Utilize fontes de vagas disponíveis por meio de integrações com APIs públicas ou serviços de emprego que permitam acesso automatizado.

Não invente vagas nem apresente dados fictícios como oportunidades reais.

Caso uma integração externa não esteja configurada ou disponível, ofereça a possibilidade de o usuário inserir uma descrição de vaga ou colar o link da oportunidade para realizar a análise de compatibilidade.

Cada vaga deve apresentar:

- Nome da empresa.
- Cargo.
- Localização.
- Modalidade: remoto, híbrido ou presencial.
- Nível de senioridade.
- Faixa salarial, quando disponível.
- Data de publicação, quando disponível.
- Descrição resumida.
- Link para candidatura.
- Percentual de compatibilidade com o currículo.

### 5.4. Sistema de compatibilidade

Crie um mecanismo inteligente de avaliação entre currículo e vaga.

A pontuação deve considerar:

- Compatibilidade de competências técnicas.
- Experiência profissional.
- Formação acadêmica.
- Senioridade.
- Ferramentas e tecnologias.
- Requisitos obrigatórios.
- Requisitos desejáveis.
- Aderência às responsabilidades do cargo.

Apresente uma pontuação de 0 a 100%.

Classifique os resultados:

- 80% a 100%: Alta compatibilidade.
- 60% a 79%: Compatibilidade moderada.
- 0% a 59%: Baixa compatibilidade.

A pontuação deve ser explicável e baseada nos requisitos identificados, não em uma avaliação arbitrária da IA.

Para cada vaga, exiba:

- Por que o candidato combina com a oportunidade.
- Competências que atendem aos requisitos.
- Requisitos parcialmente atendidos.
- Requisitos não identificados no currículo.
- Sugestões de melhoria.

Inclua filtros por cargo, localização, modalidade, senioridade e percentual mínimo de compatibilidade.

### 5.5. Detalhes da vaga

Ao selecionar uma oportunidade, apresente uma página ou painel lateral com:

- Informações completas da vaga.
- Descrição do cargo.
- Responsabilidades.
- Requisitos obrigatórios.
- Requisitos desejáveis.
- Benefícios, quando disponíveis.
- Compatibilidade com o perfil.
- Análise detalhada do matchmaking.

Inclua dois botões principais:

1. "Otimizar meu currículo para esta vaga".
2. "Acessar candidatura original".

### 5.6. Gerador de currículo ATS Friendly

Esta é a funcionalidade de maior valor da plataforma.

Quando o usuário selecionar uma vaga, a IA deverá gerar uma nova versão do currículo, adaptada especificamente àquela oportunidade.

A otimização deverá considerar:

- Palavras-chave presentes na descrição da vaga.
- Competências técnicas solicitadas.
- Terminologia utilizada pela empresa.
- Requisitos profissionais.
- Responsabilidades do cargo.
- Experiências relevantes do candidato.
- Estrutura e organização do documento.

### Regras obrigatórias de otimização ATS

O currículo gerado deverá:

- Utilizar estrutura simples e profissional.
- Evitar tabelas complexas.
- Evitar múltiplas colunas.
- Evitar elementos gráficos que prejudiquem a leitura automatizada.
- Utilizar títulos convencionais de seções.
- Apresentar palavras-chave relevantes naturalmente.
- Utilizar fontes legíveis.
- Priorizar organização textual.
- Evitar informações em cabeçalhos e rodapés que possam prejudicar a extração.
- Não incluir imagens, gráficos, barras de habilidades ou elementos decorativos desnecessários.

### Regras de integridade

A IA jamais poderá:

- Inventar experiências profissionais.
- Criar empresas fictícias.
- Alterar datas de emprego.
- Inventar formações acadêmicas.
- Adicionar certificações inexistentes.
- Declarar competências não comprovadas.
- Aumentar artificialmente o nível de experiência do candidato.

A IA poderá reorganizar, resumir e melhorar a descrição das experiências existentes, mantendo a veracidade das informações.

Quando identificar palavras-chave importantes que não estejam comprovadas no currículo, deverá sinalizá-las como lacunas, sem adicioná-las como competências do candidato.

### Visualização do currículo

Após a geração, apresente:

- Pré-visualização do novo currículo.
- Identificação da vaga para a qual foi otimizado.
- Palavras-chave incorporadas.
- Melhorias realizadas.
- Requisitos ainda não atendidos.
- Comparação entre currículo original e otimizado.

Disponibilize os botões:

- "Baixar PDF".
- "Baixar DOCX".
- "Editar currículo".
- "Gerar novamente".

O documento final deve possuir estrutura compatível com sistemas ATS e aparência profissional.

### 5.7. Histórico de análises

Crie uma área para consultar as análises realizadas durante a sessão.

Apresente:

- Currículo enviado.
- Vagas analisadas.
- Percentuais de compatibilidade.
- Currículos adaptados.
- Data das análises.

Como não haverá autenticação, mantenha os dados associados à sessão ou ao navegador do usuário, conforme a estratégia de persistência adotada.

Permita excluir os dados e iniciar uma nova análise.

## 6. Experiência do usuário e navegação

A navegação deve ser simples e intuitiva.

Sugestão de menu lateral:

- Início.
- Meu currículo.
- Encontrar vagas.
- Currículos otimizados.
- Histórico.

No topo, apresente uma identificação visual discreta do MatchCV e uma opção para limpar a sessão.

Não crie páginas de login, cadastro, recuperação de senha, autenticação social ou qualquer fluxo de criação de conta.

O usuário deve conseguir utilizar o produto imediatamente.

## 7. Arquitetura e tecnologias

Implemente a aplicação utilizando:

- React.
- TypeScript.
- Vite.
- Tailwind CSS.
- Shadcn/UI.
- Lucide React.
- Supabase ou Lovable Cloud, caso seja necessário utilizar backend.
- Inteligência artificial para análise de documentos, matchmaking e geração de currículos.

Priorize os recursos nativos disponíveis no Lovable para manter toda a implementação, configuração e manutenção dentro do ambiente Lovable.

Utilize processamento seguro no backend para operações que envolvam chaves de API e inteligência artificial.

Nunca exponha chaves privadas no frontend.

Não exija autenticação de usuário.

Se utilizar banco de dados, projete uma estrutura que permita o funcionamento sem contas individuais, utilizando identificadores de sessão ou mecanismos equivalentes.

Implemente políticas de segurança adequadas para impedir que usuários acessem dados de outras sessões.

Não armazene currículos ou informações pessoais desnecessariamente.

Informe ao usuário como seus documentos serão utilizados e permita a exclusão dos dados.

## 8. Inteligência artificial

A IA deverá atuar em três funções principais:

**Agente 1 — Analisador de currículo**

Responsável por interpretar o currículo, extrair informações estruturadas e identificar o perfil profissional.

**Agente 2 — Matchmaker de vagas**

Responsável por comparar o perfil profissional com as oportunidades disponíveis, calcular a compatibilidade e explicar os resultados.

**Agente 3 — Especialista em ATS**

Responsável por adaptar o currículo para cada oportunidade, mantendo a integridade das informações e priorizando a compatibilidade com sistemas de recrutamento automatizados.

Os agentes devem trabalhar com informações estruturadas e compartilhar os dados necessários entre as etapas.

## 9. Responsividade e acessibilidade

A aplicação deverá funcionar perfeitamente em:

- Desktop.
- Tablets.
- Smartphones.

Siga boas práticas de acessibilidade e Design Universal:

- Contraste adequado.
- Navegação por teclado.
- Estados de foco visíveis.
- Textos legíveis.
- Botões com áreas de interação adequadas.
- Rótulos claros.
- Mensagens de erro compreensíveis.
- Feedback visual para ações.
- Compatibilidade com leitores de tela.

Não utilize apenas cores para comunicar informações importantes.

## 10. Estados e feedbacks

Implemente estados completos para todas as funcionalidades:

- Estado inicial.
- Upload em andamento.
- Processamento do currículo.
- Análise concluída.
- Nenhuma vaga encontrada.
- Erro de integração.
- Erro no processamento.
- Geração do currículo.
- Download concluído.
- Histórico vazio.

Utilize Skeletons, Progress, Toasts e mensagens contextuais.

Não deixe botões sem funcionalidade.

Não apresente dados simulados como se fossem resultados reais.

## 11. Critérios de qualidade

A aplicação deverá ser desenvolvida com foco em:

- Código organizado e reutilizável.
- Componentes independentes.
- Tipagem adequada com TypeScript.
- Interface consistente.
- Boa performance.
- Segurança dos documentos enviados.
- Tratamento de erros.
- Experiência de uso fluida.
- Arquitetura preparada para futuras melhorias.

Evite funcionalidades meramente decorativas.

Todas as funcionalidades principais deverão possuir fluxos reais de funcionamento.

Caso alguma integração dependa de credenciais ou serviços externos, implemente a estrutura necessária, identifique claramente a dependência e ofereça uma alternativa funcional para o usuário não ficar bloqueado.

## 12. Diretriz final de implementação

Construa o MatchCV como um produto SaaS moderno, funcional e pronto para validação com usuários reais.

Priorize o seguinte fluxo:

1. Usuário acessa a plataforma sem login.
2. Envia seu currículo.
3. A IA analisa seu perfil.
4. A plataforma apresenta oportunidades compatíveis.
5. Usuário seleciona uma vaga.
6. A IA analisa os requisitos da oportunidade.
7. A IA gera uma versão personalizada e ATS Friendly do currículo.
8. Usuário revisa e baixa seu documento.

Antes de finalizar, verifique se a navegação, os componentes, os fluxos, os estados e as funcionalidades estão conectados corretamente.

**Importante:** Não transforme o projeto em uma landing page com botões ilustrativos. O objetivo é construir uma aplicação funcional, com inteligência artificial integrada, análise real de currículos, matchmaking explicável e geração de documentos utilizáveis.

Mantenha a identidade visual clara, elegante, minimalista e baseada em Shadcn/UI, respeitando a paleta branca e amarelo-claro definida neste documento.

Resultado final no Lovable: https://mkvagas.lovable.app/

<img width="1737" height="997" alt="image" src="https://github.com/user-attachments/assets/727b1e7d-0122-4218-ae57-6cc8e90cface" />

A aplicação ajuda o usuário a verificar vagas compatíveis com o seu curriculum e ajuda a ajustar para melhorar a oportunidade de uma futura entrevista dessas vagas compatíveis, gerando uma versão personalizada do curriculum.
```






