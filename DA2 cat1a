#include <stdio.h>
#include <string.h>
#define MAX_LEN 100
int main() {
  char str[MAX_LEN];
  int len, freq[26] = {0}, i, repeated = 0, non_repeated = 0;

  printf("Enter a string: ");
  fgets(str, MAX_LEN, stdin);

  str[strcspn(str, "\n")] = '\0';

  
  len = strlen(str);

 
  for(i = 0; i < len; i++) {
    if(str[i] >= 'a' && str[i] <= 'z') {
      freq[str[i] - 'a']++;
    }
    else if(str[i] >= 'A' && str[i] <= 'Z') {
      freq[str[i] - 'A']++;
    }
  }

  printf("Length of the string is: %d\n", len);


  printf("Word frequency is: ");
  for(i = 0; i < 26; i++) {
    if(freq[i] > 0) {
      printf("%d ", freq[i]);
    }
  }
  printf("\n"); 
  for(i = 0; i < len; i++) {
    if(str[i] >= 'a' && str[i] <= 'z') {
      if(freq[str[i] - 'a'] == 1) {
        non_repeated = str[i];
        break;
      }
      else if(freq[str[i] - 'a'] > 1 && !repeated) {
        repeated = str[i];
      }
    }
    else if(str[i] >= 'A' && str[i] <= 'Z') {
      if(freq[str[i] - 'A'] == 1) {
        non_repeated = str[i];
        break;
      }
      else if(freq[str[i] - 'A'] > 1 && !repeated) {
        repeated = str[i];
      }
    }
  }
  if(repeated) {
    printf("First repeated character is: %c\n", repeated);
  }
  else {
    printf("No repeated characters found in the string.\n");
  }
  if(non_repeated) {
    printf("First non-repeated character is: %c\n", non_repeated);
  }
  else {
    printf("No non-repeated characters found in the string.\n");
  }

  return 0;
}
