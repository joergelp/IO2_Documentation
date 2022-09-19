<p align="right">
  <a href="README.md">[EN]</a>
  <a href="README_es.md">[ES]</a>
  <a href="README_pt.md">[PT]</a>
  <a href="README_tr.md">[TR]</a>
  <a href="README_sv.md">[SV]</a>
</p>

# A especificação LTI


A especificação IMS Learning Tools Interoperability (LTI) pode ser definida como 
uma forma padronizada de integrar conteúdo de terceiros em cursos dentro de um LMS ou plataforma. 
Sem o LTI, LMS e fornecedores de conteúdo teriam que confiar em integrações *ah-hoc* 
com prejuízo à interoperabilidade e escalabilidade.
Esta especificação evoluiu de um mecanismo simples para lançar aplicações web a partir do LMS, 
para oferecer suporte a vários serviços de troca segura de dados com essas aplicações.
O LTI é um padrão suportado por todos os fornecedores de LMS de referência e, portanto, maximiza
o ganho de adaptar uma aplicação web educacional.

Atualmente, o consórcio IMS recomenda a adoção da versão 1.3. Em resumo, o LTI 1.3 usa OAuth2 
e mensagens assinadas usando JSON Web Tokens (JWTs) para autenticar os alunos com segurança 
e transmitir dados entre o LMS e a ferramenta de aprendizagem externa.
Esta versão inclui o LTI Advantage, definido como um pacote de serviços que agrega novos recursos 
para aprimorar a integração de qualquer ferramenta com qualquer LMS no núcleo do LTI 1.3. 
Os três serviços de recursos LTI são: 
 - Names and Role Provisioning Services (NRPS): concede à ferramenta acesso à lista de usuários e suas funções
    para um contexto específico (por exemplo, um curso ou grupo).
    O NRPS permite que a ferramenta externa solicite uma lista de membros do contexto que a lançou.
    Assim que a ferramenta receber a lista de membros, ela poderá ler todos os alunos e professores 
    matriculados na atividade de contexto, mesmo que ainda não tenham lançado a ferramenta. 
 - Assignment and Grade Services (AGS): permite que os professores sincronizem notas entre ferramentas 
   de terceiros e seus LMS. 
   Este serviço retorna pontuações numéricas e comentários do professor para um boletim de notas do LMS.
   Por exemplo, um professor pode ver quando um aluno iniciou uma tarefa, ou se esta foi concluída.
   O professor também pode receber uma nota, incluindo a entrada manual do professor.
 - Deep Linking (DL): oferece uma abordagem mais simplificada para adicionar links LTI a um LMS. 
   As mensagens DL permitem que ferramentas externas de aprendizagem apareçam num LMS, 
   como o fariam as ferramentas internas.
   Com o DL, as ferramentas externas de aprendizagem podem permitir que os professores configurem 
   conteúdo específico dentro da ferramenta.
   No LTI 1.1, todo o conteúdo da ferramenta tinha que ser exposto, mesmo que o professor só quisesse 
   numa aula usar um recurso específico.
   O DL permite que os professores selecionem o conteúdo de que precisam e compartilhem o link para iniciar
   esse conteúdo com o seu curso.
   Por exemplo, uma ferramenta pode permitir que um professor configure um capítulo específico de 
   um *e-book* quando seus alunos selecione um link, em vez de forçá-los a iniciar a ferramenta e navegar até esse capítulo.
    
Adotar o LTI 1.3 deve ser uma decisão cuidadosa. Para a maioria dos casos, o LTI 1.1 é suficiente
em casos de uso em que um aluno inicia uma atividade do LMS, resolve na ferramenta externa
e, em seguida, uma nota é reportada de volta ao livro de notas do LMS.
No entanto, os novos recursos LTI 1.3 podem ser aplicados em casos de uso relevantes.
Por exemplo, considerando o uso de tabelas de classificação: nomes e funções obtidos de serviços 
de provisionamento poderia ser usado para preencher tabelas de classificação com os nomes dos alunos 
antes de serem enviados pela primeira vez;
*links* diretos podem ser usados para incorporar em tabelas de classificação de conteúdo LMS 
geradas dinamicamente pela ferramenta.

