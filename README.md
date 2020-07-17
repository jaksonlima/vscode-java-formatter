# vscode-java-formatter

## https://github.com/redhat-developer/vscode-java/wiki/Formatter-settings

# Formatter settings

Para usar o formatador, você precisa de um arquivo do formatador Eclipse, como https://raw.githubusercontent.com/google/styleguide/gh-pages/eclipse-java-google-style.xml .

Defina a seguinte propriedade:

"java.format.settings.url": "https://raw.githubusercontent.com/google/styleguide/gh-pages/eclipse-java-google-style.xml",
A propriedade pode apontar para uma URL ou um caminho de arquivo local. Se o arquivo xml do formatador contiver mais perfis, você poderá definir um nome de perfil como:

"java.format.settings.profile": "GoogleStyle",
Você também pode definir as preferências de formatação no seu projeto .settings/org.eclipse.jdt.core.prefs. Ele substituirá as configurações globais de formatação.

Como isso é entediante, a melhor maneira de editar essas preferências é abrir seu projeto no Eclipse e definir as preferências de formatação para o seu projeto.

Em Eclipse, clique com botão direito em seu projeto, aberto Properties> Java Code Style> Formattere criar um novo perfil de formatação: 

Depois de salvá-lo, .settings/org.eclipse.jdt.core.prefsserá atualizado. Esse arquivo precisará ser copiado para todos os seus outros projetos no mesmo espaço de trabalho.

Não, não é uma solução ideal, mas deve ser feita apenas uma vez, a menos que você altere regularmente as configurações do formatador.
