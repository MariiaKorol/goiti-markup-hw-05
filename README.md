# goiti-markup-hw-05
/* MODAL WINDOW */

.backdrop {
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;

  transition: opacity 250ms cubic-bezier(0.4, 0, 0.2, 1);

  background-color: rgba(0, 0, 0, 0.2);
}

.modal {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%) scale(1);
  min-width: 528px;
  min-height: 581px;
  border-radius: 4px;

  transition: transform 500ms cubic-bezier(0.4, 0, 0.2, 1);

  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2), 0 1px 1px rgba(0, 0, 0, 0.14);
  background-color: var(--white-color);
}

.backdrop.is-hidden .modal {
  transform: scale(1.1) translate(-50%, -50%);
}

.close-button {
  position: absolute;
  top: 8px;
  right: 8px;
  width: 30px;
  height: 30px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  border: 1px solid rgba(0, 0, 0, 0.1);
  border-radius: 50%;
  background-color: inherit;
}