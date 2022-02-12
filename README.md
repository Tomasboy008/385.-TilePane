# 385.-TilePane
Configuração parecida com FlowPane
package layout;
INICIO
____________________________________
import java.util.ArrayList;
import java.util.List;

import javafx.geometry.Insets;
import javafx.geometry.Orientation;
import javafx.geometry.Pos;
import javafx.scene.layout.TilePane;

public class TesteTilePane extends TilePane{

		public TesteTilePane() {

			List<Quadrado> quadrados = new ArrayList<>();
			
			for (int i = 1; i < 10; i++) {
				quadrados.add(new Quadrado(i * 10));
			}
			setPadding(new Insets(20, 10, 20, 10));
			setVgap(10);
			setHgap(10);
			
			setOrientation(Orientation.VERTICAL);
			setTileAlignment(Pos.BOTTOM_RIGHT);
			getChildren().addAll(quadrados);
		 }		
}
![image](https://user-images.githubusercontent.com/95525963/153687167-d12cba56-3841-4727-8b29-19911573797a.png)
