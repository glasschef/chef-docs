.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

The syntax for the ``control_group`` method is as follows:

.. code-block:: ruby

   control_group "name" do
     control "name" do
       it "should do something" do
         expect(something).to/.to_not be_something
       end
     end
     control "name" do
       ...
     end
     ...
   end

where:

* ``control_group`` groups one (or more) ``control`` blocks
* ``"name"`` is the unique name for the ``control_group``; the |chef client| will raise an exception if duplicate ``control_group`` names are present
* ``control`` defines each individual audit within the ``control_group`` block. There is no limit to the number of ``control`` blocks that may defined within a ``control_group`` block
