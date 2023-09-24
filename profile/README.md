<!-- The banner designed by https://github.com/iLillie -->
<!-- TODO: replace with a thinner banner, where instead of stretching the entire image,
     only the black sides are stretched. I think it would look cooler, but I don't know
     SVG! -->
![251627673-957d5ef4-6e2e-4333-940a-3526b530d4e2](https://github.com/Norske-Nokkelsnikere/proposed.github/assets/24797093/9863e302-062a-4822-b97a-8abbd2c66889)

<div align=center><h1>Norske Nøkkelsnikere</h1></div>
Norske Nøkkelsnikere is a Norwegian CTF team

# Writeups
<!--

;; This is just a silly little elisp program I wrote to generate an
;; index. I won't get mad if you replace or delete this haha ;)
;;
;; I'm sure this could be solved with a shellscript one-liner...
(save-excursion
 ;; Delete old index, super brittle code....
 (forward-line)
 (end-of-line)
 (delete-region (point) (point-max))
 (newline)

 ;; Generate new index
 (->>
  ;; Might be better to use `$ git ls-files`
  (directory-files-recursively (concat default-directory "writeups") "")
  (mapcar (-rpartial 'file-relative-name default-directory))gcc

  ;; The following line is equivalent to
  ;; (seq-filter (-compose 'not (-partial 's-prefix? ".")))
  (seq-remove (-partial 's-prefix? "."))
  (seq-remove (-partial 'equal "README.md"))
  (mapcar (lambda (path) (concat "- [" path "]" "(" path ")")))
  (s-join "\n")
  insert))
 -->
- [writeups/2023/tjctf-2023/web-ez-sql.md](writeups/2023/tjctf-2023/web-ez-sql.md)
- [writeups/2023/uiuctf-2023/misc-vimjail.md](writeups/2023/uiuctf-2023/misc-vimjail.md)
