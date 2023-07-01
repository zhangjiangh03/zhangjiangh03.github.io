---
title: 【期末-C语言】C语言图形输出题
date: 2023-07-01 11:40:36
categories: 大学
tags: 
- 大一
- 期末
- C语言
- 图形输出
---

```text
$ $ $ $ $
$ $ $ $ $
$ $ $ $ $
$ $ $ $ $
$ $ $ $ $
```

```c
#include <stdio.h>

int main() {
	int i, j;

	for (i = 0; i < 5; i++) {
		for (j = 0; j < 5; j++) {
			printf("$");
		}
		printf("\n");
	}

	return 0;
}
```

```text
$ $ $ $ $
  $ $ $ $ $
    $ $ $ $ $
      $ $ $ $ $ 
        $ $ $ $ $
```

```c
#include <stdio.h>

int main() {
	int i, j, k;

	for (i = 0; i < 5; i++) {
		for (j = 0; j < i; j++) {
			printf("  ");
		}
		for (k = 0; k < 5; k++) {
			printf("$ ");
		}
		printf("\n");
	}

	return 0;
}
```

```text
$
$ $ $
$ $ $ $ $
$ $ $ $ $ $ $
$ $ $ $ $ $ $ $ $
```

```c
#include <stdio.h>

int main() {
	int i, j, k;

	for (i = 0; i < 5; i++) {
		for (j = 0; j < 2 * i + 1; j++) {
			printf("$ ");
		}
		printf("\n");
	}

	return 0;
}
```

```text
        $ $ $ $ $
      $ $ $ $ $
    $ $ $ $ $
  $ $ $ $ $   
$ $ $ $ $
```

```c
#include <stdio.h>

int main() {

    for (int i = 0; i < 5; i++) {
        for (int j = 5; j > i + 1; j--) {
            printf("  ");
        }
    
        for (int k = 0; k < 5; k++) {
            printf("$ ");
        }
        printf("\n");
    }

    return 0;
}
```

```text
      $  
    $ $ $ 
  $ $ $ $ $
$ $ $ $ $ $ $
  $ $ $ $ $
    $ $ $
      $
```

```c
#include <stdio.h>

int main() {
    for (int i = 0; i < 4; i++) {
        for (int j = 4; j > i + 1; j--) {
            printf("  ");
        }

        for (int k = 0; k < 2 * i + 1; k++) {
            printf("$ ");
        }
        printf("\n");
    }

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < i + 1; j++) {
            printf("  ");
        }

        for (int j = 0; j < 5 - 2 * i; j++) {
            printf("$ ");
        }
        printf("\n");
    }
    return 0;
}
```

```text
$ $ $ $ $
  $ $ $
    $
  $ $ $
$ $ $ $ $
```

```c
#include <stdio.h>

int main() {

    for (int i = 1; i <= 3; i++) {
        for (int j = 1; j <= 2 * i - 2; j++) {
            printf(" ");
        }

        for (int k = 0; k < 7 - 2 * i; k++) {
            printf("$ ");
        }
        printf("\n");
    }

    for (int i = 1; i <= 2; i++) {
        for (int j = 1; j <= 4 - 2 * i; j++) {
            printf(" ");
        }

        for (int k = 0; k <= 2 * i; k++) {
            printf("$ ");
        }
        printf("\n");
    }

    return 0;
}
```