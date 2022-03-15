# GOF Estrutural Bridge

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 09/02/2022 | Criação do Documento | Liverson Paulo e Giulia Lobo | Lucas Andrade e Dafne Moretti |

## Introdução e metodologia

Este padrão de projeto vai permitir que uma classe grande ou classes que estão ligadas intimamente sejam divididas em duas hierarquias separadas, sendo elas a abstração e a implementação. Elas podem ser  desenvolvidas de formas independentes umas das outras.

Ao trocar herança por composição do objeto, esse formato tenta evitar com que haja heranças que crescem de maneira exponencial.

Basicamente este método extrai uma das dimensões de uma hierarquia em uma classe separada, ao invés de ter todos os seus estados e comportamentos dentro de uma classe

### Exemplo de execução sem Bridge

![](../../assets/images/bridgept1.png)
</br> Figura 1 - Exemplo de execução sem Bridge. Fonte: [https://refactoring.guru/pt-br/design-patterns/bridge](https://refactoring.guru/pt-br/design-patterns/bridge)

### Exemplo de execução com Bridge

![](../../assets/images/bridgept2.png)
</br> Figura 2 - Exemplo de execução com Bridge. Fonte: [https://refactoring.guru/pt-br/design-patterns/bridge](https://refactoring.guru/pt-br/design-patterns/bridge)

### Exemplo de código usando o padrão Bridge

Abaixo, temos um exemplo de implementação do padrão GoF Bridge em Java:

``` 
public interface Device {
    boolean isEnabled();

    void enable();

    void disable();

    void setVolume(int percent);

    void setChannel(int channel);

} 
```

A interface Device se comporta como uma interface comum para todos os dispositivos. Nela, temos as funções desempenhadas por cada dispositivo.

```
public class Tv implements Device {
    private boolean on = false;
    private int volume = 30;
    private int channel = 1;

    @Override
    public boolean isEnabled() {
        return on;
    }

    @Override
    public void enable() {
        on = true;
    }

    @Override
    public void disable() {
        on = false;
    }


    @Override
    public void setVolume(int volume) {
        if (volume > 100) {
            this.volume = 100;
        } else if (volume < 0) {
            this.volume = 0;
        } else {
            this.volume = volume;
        }
    }


    @Override
    public void setChannel(int channel) {
        this.channel = channel;
    }
}
```

A classe TV vai ser responsável por implementar a classe device, apresentando as funções comuns entre os devices. Dessa forma, é possível passar um objeto do tipo device para uma função, aumentando o reaproveitamento de código.

```
public class Radio implements Device {
    private boolean on = false;
    private int volume = 30;
    private int channel = 1;

    @Override
    public boolean isEnabled() {
        return on;
    }

    @Override
    public void enable() {
        on = true;
    }

    @Override
    public void disable() {
        on = false;
    }

    @Override
    public void setVolume(int volume) {
        if (volume > 100) {
            this.volume = 100;
        } else if (volume < 0) {
            this.volume = 0;
        } else {
            this.volume = volume;
        }
    }

    @Override
    public void setChannel(int channel) {
        this.channel = channel;
    }
    }
}
```
A classe rádio também implementa a interface Device, pois é um tipo de Device e apresenta características e funcionalidades semelhantes à TV. Todavia, ela implementa os métodos também presentes na TV de forma diferente. 

```
public class Main {
    public static void main(String[] args) {
        testDevice(new Tv());
        testDevice(new Radio());
    }

    public static void testDevice(Device device) {
        if (!device.isEnabled()) {
            device.enable()
        }
        device.setVolume(30)
        device.setChannel(10)
        device.disable()
    }
}
```

Acima, temos um exemplo de utilização do padrão Bridge, onde são passadas para a chamada da função os objetos que são instâncias de classes que implementam a interface. Dessa forma, é possível utilizar os métodos presentes na interface tanto para a TV quanto para o rádio.

## Conclusão

O GOF Estrutural Bridge tem potencial para se encaixar no nosso projeto, pode ajudar em principalmente em relação aos lanches já que podem ter vários atributos diferentes dentro deles.

## Bibliografia

Bridge. Disponível em: https://refactoring.guru/pt-br/design-patterns/bridge. Acesso em: 24/02/2022