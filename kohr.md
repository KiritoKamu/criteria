# Критерии Кохрена

Если размеры выборок одинаковы, можем использовать для равенства дисперсий критерий Кохрена.

# Определения

$$G = \frac{S^2_{max}}{S^2_1 + S^2_2 + ... + S^2_m}$$

В предположении, что нуль-гипотеза равна, распределение этой статистики зависит только от числа степеней свободы $$k = n - 1$$ и числа выборок $$m$$.

По таблице находим критическую точку $$G_{кр} = G(\alpha, k, m)$$. Если $$G < G_{кр}$$, то $$H_0$$ принимается, в противном случае - отвергаем.

Если гипотеза о равенстве дисперсий для всех выборок принимается, то в качестве оценки этой общей дисперсии можно использовать величину $$S^2$$.

Критические значения можно найти, пользуясь таблицами F-распределения (при $$n \geq 20$$) с помощью соотношения:

$$G(p, k, m) = \frac{F_{1+\frac{1}{k}-\frac{p}{k}}[m - 1; (m - 1)(k - 1)]}{k - 1 + F_{1+\frac{1}{k}-\frac{p}{k}}[m - 1; (m - 1)(k - 1)]}$$,

где $$F_\gamma[f_1, f_2]$$ - $$\gamma$$ - квантиль $$F$$ - распределения с $$f_1$$ и $$f_2$$ степенями свободы.

# Примеры

Четыре выборки:

$$x_1 = {3, 4, 5, 6, 7}$$;
$$x_2 = {2, 8, 9, 11, 15}$$;
$$x_3 = {9, 11, 15, 20, 28}$$;
$$x_4 = {4, 6, 8, 10, 16}$$;

Проверим нуль-гипотезу равенства дисперсий по критерием Кохрена при доверительной вероятности $$p = 0.95$$.

Для вычисления статистики найдем сумму оценок дисперсии:

$$\sum S^2_i = 2.5 + 22.5 + 58.3 + 21.2 = 104.4$$;

При этом:

$$\max s^2_i = 58.3$$

Тогда по формуле:

$$G = \frac{58.3}{104.5} = 0.558$$;

По табличным значениям для $$n = 5, k = 4, p = 0.95$$ имеется $$G = 0.721$$.

Тогда $$G = 0.558 < 0.721$$ нуль-гипотеза не отклоняется.

### [Вернуться на главную](/)
