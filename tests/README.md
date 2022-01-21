
#  Examples - README


To reproduce the examples shown in our paper, execute the
following commands (ensure polyclip executable is in test folder):

- `polyclip Fig8-P.poly Fig8-Q.poly Fig8-R.poly`
- `polyclip Fig12-P.poly Fig12-Q.poly Fig12-R.poly`
- `polyclip Fig14-P.poly Fig14-Q.poly Fig14-R.poly`
- `polyclip Fig15-P.poly Fig15-Q.poly Fig15-R.poly`
- `polyclip Fig16-P.poly Fig16-Q.poly Fig16-R.poly`
- `polyclip Fig17-P.poly Fig17-Q.poly Fig17-R.poly`
- `polyclip Fig18-P.poly Fig18-Q.poly Fig18-R.poly`
- `polyclip Fig19-P.poly Fig19-Q.poly Fig19-R.poly`

## Example in Figures 20:

  1) to compute the union of the 5 elementary school districts

  - `polyclip -union Fig20-E1.poly Fig20-E2.poly Fig20-E12.poly`
  - `polyclip -union Fig20-E12.poly Fig20-E3.poly Fig20-E123.poly`
  - `polyclip -union Fig20-E123.poly Fig20-E4.poly Fig20-E1234.poly`
  - `polyclip -union Fig20-E1234.poly Fig20-E5.poly Fig20-E.poly`
  - `Fig20-E.poly` will contain the resulting polygon
  

  2) to compute the union of the 3 middle school districts

  - `polyclip -union Fig20-M1.poly Fig20-M2.poly Fig20-M12.poly`
  - `polyclip -union Fig20-M12.poly Fig20-M3.poly Fig20-M.poly`
  - `Fig20-M.poly` will contain the resulting polygon

  3) to compute the union of the 2 high school districts

  - `polyclip -union Fig20-H1.poly Fig20-H2.poly Fig20-H.poly`
  - `Fig20-H.poly` will contain the resulting polygon

  4) to intersect the three union polygons

  - `polyclip Fig20-E.poly Fig20-M.poly Fig20-EM.poly`
  - `polyclip Fig20-EM.poly Fig20-H.poly Fig20-R.poly`
  - `Fig20-R.poly` will contain the final result

## Filling degenerate hole tests
  - `polyclip -union ChessBoard1-P.poly ChessBoard1-Q.poly ChessBoard1-R.poly`
  - `polyclip -union ChessBoard2-P.poly ChessBoard2-Q.poly ChessBoard2-R.poly`
  - `polyclip -union ChessBoard3-P.poly ChessBoard3-Q.poly ChessBoard3-R.poly`
  - `polyclip -union ChessBoard4-P.poly ChessBoard4-Q.poly ChessBoard4-R.poly`
  - `polyclip -union ChessBoard5-P.poly ChessBoard1-Q.poly ChessBoard5-R.poly`
    