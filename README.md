# ATLAS — PWA pessoal de treino e nutrição

## Instalação no iPhone

1. Publique **todo o conteúdo desta pasta** em um host HTTPS estático (Netlify Drop, por exemplo). Não envie apenas o index.html.
2. Abra a URL publicada no Safari do iPhone.
3. Compartilhar → Adicionar à Tela de Início → Adicionar (se disponível, ativar "Abrir como App").
4. Abra o ícone ATLAS. Após o primeiro carregamento, a interface pode funcionar offline.

## Funções

- Rotina inicial: segunda peito/costas, terça HYROX, quarta braços, quinta HYROX, sexta upper, sábado pernas/ombros e domingo descanso.
- Registro de séries marcadas, cargas e repetições, histórico e gráfico de cargas.
- Cronômetro de descanso.
- Diário alimentar por data com alimentos por 100 g ou porção e somas de kcal, proteína, carboidrato e gordura.
- Metas editáveis, backup JSON e restauração.

- Editor em Ajustes: renomear treinos, trocar os dias, adicionar, remover, alterar e reordenar exercícios, séries, repetições e carga inicial. O histórico de sessões é mantido.

## Notas importantes

- HYROX 2 foi colocado no dia 7 **provisoriamente**, pois a segunda posição semanal não foi especificada. O dia 4 substitui REST / BOXING do PDF.
- O programa foi transcrito do PDF, separando exercícios apresentados com barras (/) em linhas independentes.
- As metas de nutrição são exemplos, não recomendações individualizadas. Os valores nutricionais são inseridos pelo usuário; não há banco externo de alimentos nem reconhecimento automático de texto/foto.
- Os dados ficam no `localStorage` do navegador. Não há sincronização em nuvem, conta ou garantia de preservação caso dados do site sejam apagados. Exporte backups frequentemente.
- Para mudar a programação semanal, edite o array `workouts` no início do script de `index.html` e publique uma nova versão (novas instalações). A data de início do ciclo é ajustável no app.
- Em alguns iPhones, arquivos baixados em JSON são salvos em Arquivos; a exportação depende do Safari.

## Agenda semanal atualizada
- Segunda: Chest / Back
- Terça: HYROX 1
- Quarta: Arms
- Quinta: HYROX 2
- Sexta: Upper
- Sábado: Shoulders / Legs
- Domingo: descanso

O aplicativo agora utiliza os dias reais da semana e migra automaticamente a ordem antiga dos treinos salvos.
