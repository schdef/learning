
public class Tree {
	Node root;
	
	public boolean insert(int val) {
		if (root == null) {
			root = new Node(val);
			return true;
		} else {
			return root.insert(val);
		}
	}
	
	public boolean find(int val) {
		if (this.root == null) {
			return false;
		} else {
			return this.root.find(val);
		}
	}
	
	
	private class Node {
		
		private Node leftNode;
		private Node rightNode;
		int data;
		
		public Node(int val) {
			this.data = val;
		}
		
		public boolean insert(int val) {
			if(val < this.data) {
				if (this.leftNode == null) {
					this.leftNode = new Node(val);
					return true;
				} else {
					return this.leftNode.insert(val);
				}
			} else if (val > this.data) {
				if (this.rightNode == null) {
					this.rightNode = new Node(val);
					return true;
				} else {
					return this.rightNode.insert(val);
				}
			}
			
			return false;
		}
		
		private boolean find(int val) {
			if(this.data == val) {
				return true;
			} else if(val < this.data && this.leftNode != null) {
				return this.leftNode.find(val);
			} else if(val > this.data && this.rightNode != null) {
				return this.rightNode.find(val);
			}
			
			return false;
		}
		
	}
}
