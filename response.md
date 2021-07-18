Reponse 1 : 

   . La fonction foo()  prends en parametre un ensemble des intervalles  et à la sortie retourne  l'union de ces intervales.

Reponse 2:
  .public function  getArray()
  {
          $data=[[0, 3], [6, 10]];
        $n = 0; $len = count($data);
        for ($i = 1; $i < $len; ++$i)
        {
            if ($data[$i][0] > $data[$n][1] + 1)
                $n = $i;
            else
            {
                if ($data[$n][1] < $data[$i][1])
                    $data[$n][1] = $data[$i][1];
                    unset($data[$i]);
            }
        }
        $data = array_values($data);
    }


Reponse 3 :

  . J'ai implémenté la fonction en 45 minutes. c'est je veux amélioré ça.
