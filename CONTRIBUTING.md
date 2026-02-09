# Guia de Contribuição

Obrigado por considerar contribuir para o Selenium Test Framework! Este documento fornece diretrizes para contribuições.

## 📋 Código de Conduta

### Nosso Compromisso
Nos comprometemos em proporcionar um ambiente acolhedor e inclusivo para todos.

### Nossos Padrões
- Use linguagem acolhedora e inclusiva
- Seja respeitoso com pontos de vista e experiências divergentes
- Aceite críticas construtivas
- Concentre-se no que é melhor para a comunidade

## 🚀 Como Contribuir

### Reportando Bugs

Antes de abrir um relatório de bug, verifique se o problema foi relatado. Se você encontrar um bug:

1. **Use um título descritivo**
2. **Descreva os passos reprodutíveis**
3. **Forneça exemplos específicos**
4. **Descreva o comportamento observado**
5. **Descreva o comportamento esperado**

### Sugerindo Enhancements

Se você tem uma sugestão de melhoria:

1. **Use um título descritivo**
2. **Forneça uma descrição detalhada da melhoria sugerida**
3. **Liste alguns exemplos de como essa melhoria seria usada**

### Pull Requests

- Preencha o template fornecido
- Siga os padrões de codificação do projeto
- Inclua testes apropriados
- Atualize a documentação relevante

## 🎨 Padrões de Código

### Nomenclatura
- **Pacotes**: `com.automation.{funcionalidade}` (lowercase)
- **Classes**: PascalCase (ex: `GoogleSearchPage`)
- **Métodos**: camelCase (ex: `searchFor()`)
- **Constantes**: UPPER_SNAKE_CASE

### Estrutura
```java
// 1. Comentário de classe
public class MyClass {
    // 1. Constantes
    private static final String CONSTANT = "value";
    
    // 2. Variáveis
    private String variable;
    
    // 3. Construtor
    public MyClass() {}
    
    // 4. Métodos públicos
    public void publicMethod() {}
    
    // 5. Métodos protegidos
    protected void protectedMethod() {}
    
    // 6. Métodos privados
    private void privateMethod() {}
}
```

### Logging
```java
// Use logger da classe
private static final Logger logger = LogManager.getLogger(MyClass.class);

// Em métodos
logger.info("Informação sobre o passo executado");
logger.warn("Aviso sobre comportamento inesperado");
logger.error("Erro capturado com exceção", exception);
```

### Anotações Allure
```java
@Epic("Feature Principal")
@Feature("Subfuncionalidade")
@Story("O que o usuário quer fazer")
@Description("Descrição detalhada do teste")
@Severity(SeverityLevel.CRITICAL)
public void testExample() {}
```

## 📦 Processo de Desenvolvimento

1. **Fork** o repositório
2. **Clone** seu fork: `git clone https://github.com/seu-usuario/selenium-test-framework.git`
3. **Crie uma branch**: `git checkout -b feature/sua-feature`
4. **Faça as mudanças**
5. **Commit**: `git commit -m "Descrição clara da mudança"`
6. **Push**: `git push origin feature/sua-feature`
7. **Abra um Pull Request**

## ✅ Checklist antes de submeter PR

- [ ] Código segue os padrões do projeto
- [ ] Adicionei testes para minhas mudanças
- [ ] Todos os testes passam localmente (`mvn clean test`)
- [ ] Atualizei a documentação relevante
- [ ] Sem warnings do Maven
- [ ] Meu código não tem code smells

## 📚 Stack Tecnológico

- **Java 11+**
- **Maven 3.6+**
- **Selenium 4.x**
- **JUnit 4**
- **Allure 2.x**
- **Log4j 2**

## 🐛 Relatando Vulnerabilidades

Não abra issues públicas para vulnerabilidades. Em vez disso, reporte para cassiolinden@email.com

## 🎯 Áreas onde Contribuições são Bem-vindas

- Novos Page Objects para diferentes aplicações
- Melhorias em relatórios e documentação
- Testes adicionais
- Refatoração de código
- Otimizações de performance
- Suporte para novos browsers

## ❓ Perguntas?

Abra uma issue com a tag `[QUESTION]` ou entre em contato!

Obrigado por contribuir! 🙏