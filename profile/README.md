<!-- The banner designed by https://github.com/iLillie -->
<!-- TODO: replace with a thinner banner, where instead of stretching the entire image,
     only the black sides are stretched. I think it would look cooler, but I don't know
     SVG! -->
<!--![251627673-957d5ef4-6e2e-4333-940a-3526b530d4e2](https://github.com/Norske-Nokkelsnikere/proposed.github/assets/24797093/9863e302-062a-4822-b97a-8abbd2c66889)-->

<svg width="711" height="334" viewBox="0 0 711 334" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M181.485 36C182.808 36 184.077 36.5242 185.014 37.4579L355.723 207.531V300H280.376C277.614 300 275.376 297.761 275.376 295V242.7C275.376 241.371 274.846 240.096 273.904 239.157L151.788 117.534C150.851 116.601 149.582 116.077 148.259 116.077H129.347C126.586 116.077 124.347 118.315 124.347 121.077V295C124.347 297.761 122.109 300 119.347 300H49C46.2386 300 44 297.761 44 295V41C44 38.2386 46.2386 36 49 36H181.485Z" fill="#FF3A3A"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M275.376 127.982L355.723 207.7V36H280.376C277.614 36 275.376 38.2386 275.376 41V127.982Z" fill="white"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M435.347 208.484L355 128.5V300H430.35C433.111 300 435.35 297.761 435.35 295L435.347 208.484Z" fill="white"/>
<path d="M529.238 300C527.915 300 526.647 299.476 525.709 298.542L355 128.469V36H430.347C433.109 36 435.347 38.2386 435.347 41V93.2999C435.347 94.6294 435.877 95.9043 436.819 96.8425L558.936 218.466C559.873 219.399 561.141 219.923 562.464 219.923H581.376C584.137 219.923 586.376 217.685 586.376 214.923V41C586.376 38.2386 588.614 36 591.376 36H661.723C664.485 36 666.723 38.2386 666.723 41V295C666.723 297.761 664.485 300 661.723 300H529.238Z" fill="#505FE0"/>
</svg>

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
