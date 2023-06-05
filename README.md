Gra leży skompilowana w folderze app pod nazwą Main.exe. Aby ją uruchomić wystarczy z wnętrza folderu app
wpisać w terminalu .\Main.exe.

Jeśli jednak gra wymaga skompilowania, wtedy:
1.Rozpakuj folder "prerequisites" na dysku C.
2.Dodaj ścieżkę C:\mingw64\bin do zmiennych systemowych.
3.Wejdź do folderu app i wykonaj komendę:
g++ -Iinclude -Iinclude/SDL2 -Iinclude/headers -Llib -o Main src/*.cpp -lmingw32 -lSDL2main -lSDL2 -lSDL2_image
Powinien poprawnie wygenerować się plik Main.exe.
3.Wpisz .\Main.exe w terminalu i gra powinna się uruchomić.