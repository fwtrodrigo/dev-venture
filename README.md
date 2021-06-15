# Registro Dev-Venture

Atividades realizadas durante o bootcamp Dev Venture


# Dev-Venture

- Atividades
    - [Hackerrank](https://www.hackerrank.com/challenges/simple-array-sum)
        - Soma dos valores de um array

            ```kotlin
            fun simpleArraySum(ar: Array<Int>): Int = ar.sum()
            ```

    - [Koans](https://play.kotlinlang.org/koans/)
        - [Introdução](https://play.kotlinlang.org/koans/Introduction)
            - [Named arguments](https://play.kotlinlang.org/koans/Introduction/Named%20arguments/Task.kt)

                ```kotlin
                fun joinOptions(options: Collection<String>) =
                options.joinToString(prefix= "[", postfix = "]")
                ```

            - [Default arguments](https://play.kotlinlang.org/koans/Introduction/Default%20arguments/Task.kt)

                ```kotlin
                fun foo(name: String, number: Int = 42, toUpperCase: Boolean = false) =
                (if (toUpperCase) name.uppercase() else name) + number
                ```

            - [Triple-quoted strings](https://play.kotlinlang.org/koans/Introduction/Triple-quoted%20strings/Task.kt)

                ```kotlin
                val tripleQuotedString = """
                #question = "$question"
                #answer = $answer""".trimMargin("#")
                ```

            - [String templates](https://play.kotlinlang.org/koans/Introduction/String%20templates/Task.kt)

                ```kotlin
                fun getPattern(): String = """\d{2} $month \d{4}"""
                ```

            - [Nullable types](https://play.kotlinlang.org/koans/Introduction/Nullable%20types/Task.kt)

                ```kotlin
                fun sendMessageToClient(client: Client?, message: String?, mailer: Mailer) {
                    val personalInfo = client?.personalInfo
                    val email = personalInfo?.email
                   
                    if(email == null || message == null) return
                    
                    mailer.sendMessage(email, message)
                }
                ```

            - [Nothing type](https://play.kotlinlang.org/koans/Introduction/Nothing%20type/Task.kt)

                ```kotlin
                fun failWithWrongAge(age: Int?): Nothing  {
                		throw IllegalArgumentException("Wrong age: $age")
                }
                ```

            - [Lambdas](https://play.kotlinlang.org/koans/Introduction/Lambdas/Task.kt)

                ```kotlin
                fun containsEven(collection: Collection<Int>): Boolean =
                        collection.any { it % 2 == 0 }
                ```

- Desafios

    [Aplicativo Jogue Os Dados](https://github.com/fwtrodrigo/jogar_dados)

    [Aplicativo Layout Calculadora](https://github.com/fwtrodrigo/dev-venture-calc-layout)
